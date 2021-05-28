# act1

```
SceneSetup.act1();
```

(...300)

n: E ESTA É A ANSIEDADE DO HUMANO

n: _TU_ ÉS A ANSIEDADE

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Oh olá! Estamos de volta aqui?

`hong({eyes:"0_neutral"})`

n: O TEU TRABALHO É PROTEGER O TEU HUMANO DO *PERIGO*

`bb({eyes:"look", mouth:"small_lock"})`

n: NA VERDADE, REPETIR ESTE JOGO ESTÁ A COLOCÁ-LO EM *PERIGO*

n: RÁPIDO, AVISA-O!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Humano! Ouve, estamos em perigo! O jogador...

[...vai-nos torturar outra vez!](#act1_replay_torture)

[...não vai encontrar um final alternativo!](#act1_replay_alternate)

[...vai ter dissonância ludonarrativa!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Vai fazer-nos chorar!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Vai fazer-nos destruir o teu telefone por te ter dado um ataque de pânico!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: Vai fazer-nos *NÃO* bater no anfitrião da festa!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Vai fazer-nos dar um soco ao anti-vilão empático, o anfitrião da festa!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Bem, pelo menos há a possibilidade de não saltarmos do tel--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: VAI FAZER-NOS SALTAR DO TELHADO. 
{{/if}}

`bb({body:"fear"});`

b: TODAS ESTAS NOVAS COISAS TERRÍVEIS VÃO ACONTECER-NOS, E DEPOIS VAMOS--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Claro, a história como um *todo* é a mesma, mas cada capítulo tem dois finais possíveis, mais todos os diálogos ramificados opcio--

`bb({body:"fear"});`

b: O jogador vai ficar desapontado, fechar este separador, excluir o nosso software e depois vamos--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Um obsceno-o quê?

`bb({eyes:"normal"});`

b: O ponto alto da história era sobre como tu podes *ESCOLHER* construir uma colaboração saudável com o teu medo,

`bb({eyes:"normal_right"});`

b: Mas repetir o jogo dará a mesma história, implicando que as tuas *ESCOLHAS* não importam,

`bb({eyes:"narrow_eyebrow"});`

b: Mostrando assim uma contradição entre a mensagem do jogo e a mecânica,

`bb({eyes:"fear"});`

b: Desvendando assim o tecido deste universo narrativo,

`bb({body:"fear"});`

b: E depois vamos--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: MORREEEEEEEEER

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: Ok, vamos voltar à personagem.

```
Game.clearText();
```

n4: (DEIXA A _TUA_ ANSIEDADE BLÁ BLÁ BLÁ MAIS SEMELHANTE AO _TEU_ MEDO BLÁ BLÁ SABES COMO É)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Oh ótimo, o meu lobo está de volta. Faaaaantástico.

`hong({eyes:"0_neutral"})`

n: O TEU TRABALHO É PROTEGER O TEU HUMANO DO *PERIGO*

`bb({eyes:"look", mouth:"small_lock"})`

n: DE FACTO, AQUELA SANDUÍCHE ESTÁ A PÔ-LO EM *PERIGO* AGORA MESMO

n: RÁPIDO, AVISA-O!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Humano! Ouve, estamos em perigo! O perigo é...

`bb({body:"squeeze"})`

n4: (DEIXA A _TUA_ ANSIEDADE VIR À TONA! ESCOLHE O QUE É MAIS SEMELHANTE AO QUE O _TEU_ MEDO TE DIZ)

(#act1_normal_choice)

# act1_normal_choice

[Estamos a almoçar sozinhos! Outra vez!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Não somos produtivos enquanto comemos!](#act1a_productive) `bb({body:"squeeze_talk"})`

[O pão branco faz-nos mal!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Sabes que a solidão está associada à morte prematura tanto quanto fumar 15 cigarros por dia?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"});`

h: Hum, obrigado por citares as tuas referências, mas--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: O que significa que, se não convivermos com alguém *agora*, vamos-

`bb({body:"panic"})`

b: MORREEEEEEEEER

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: USASTE O *MEDO DE NÃO SER AMADO*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Pega já no teu portátil e trabalha um bocado!

`hong({eyes:"0_annoyed"});`

h: Hum, prefiro não deixar cair migalhas no meu tecla--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Se não estivermos a contribuir para a sociedade, então somos um parasita da sociedade!

b: A sociedade irá ao médico da sociedade pedir medicação para matar os parasitas da sociedade, e nós vamos--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: MORREEEEEEEEER

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: USASTE O *MEDO DE SER MÁ PESSOA*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Esses estudos foram replica--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: O trigo processado vai aumentar o açúcar no nosso sangue, e depois vai ser preciso amputar todos os nossos membros e depois vamos-

`bb({body:"panic"})`

b: MORREEEEEEEEER

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: USASTE O *MEDO DE SER MAGOADO*

(#act1b)

# act1b

n: É SUPER EFICAZ

`bb({mouth:"smile", eyes:"smile"});`

b: Vês, humano? Eu sou o teu fiel Lobo de Guarda!

`bb({body:"pride_talk"});`

b: Confia na tua intuição! Os teus sentimentos são sempre válidos!

`bb({body:"pride"});`

n: BAIXA A BARRA DE ENERGIA DO TEU HUMANO ATÉ ZERO

n: PARA PROTEGERES AS SUAS NECESSIDADES FÍSICAS + SOCIAIS + MORAIS, PODES USAR:

n: *MEDO DE SER MAGOADO* #harm#

n: *MEDO DE NÃO SER AMADO* #alone#

n: E *MEDO DE SER MÁ PESSOA* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (DICA: ESCOLHE AS OPÇÕES QUE ATINJAM PESSOALMENTE OS TEUS MEDOS MAIS PROFUNDOS E OBSCUROS!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: sabes, talvez seja altura de verificar o meu telemóvel.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: PROTEGE O TEU HUMANO

n: DO MUNDO. DAS OUTRAS PESSOAS. DE SI MESMO.

n: BOA SORTE

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: RONDA UM: *LUTA!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Huh. O feed do Facebook diz que vai haver uma festa neste fim-de-semana.

`bb({eyes:"uncertain"});`

b: Esse esquisitóide não dá uma festa *todos* os fins-de-semana?

`bb({eyes:"uncertain_right"});`

b: Que vazio interior está a tentar preencher? Deve estar profundamente ^fodido^ por dentro!

`hong({eyes:"surprise"});`

h: Além disso, recebi um convite?

`bb({eyes:"fear", mouth:"normal"});`

b: Pois bem!

[Diz sim ou vamos morrer de solidão!](#act1c_loner)

[Diz não, está cheio de drogas venenosas!](#act1c_drugs)

[Ignora, nós só tornamos as festas deprimentes.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: Quinze cigarros por dia, humano! Quinze!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: Depois ninguém vai aparecer no nosso funeral, vão deitar as nossas cinzas ao oceano e vamos ser comidos por uma baleia,
{{/if}}

{{if !_.fifteencigs}}
b: e nós depois vamos ser COCÓ DE BALEIA!
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: Então, sim, devemos ir à festa!
{{/if}}

{{if _.parasite}}
b: Basta trazer o portátil para que possamos trabalhar e não sermos um parasita da sociedade. 
{{/if}}

{{if _.whitebread}}
b: Desde que não sirvam PÃO BRANCO
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: DEUS. Se isso te fizer calar a boca, tudo bem.

h: Eu vou dizer que sim.

{{if _.whalepoop}}
b: Cocó de baleia, humano! Cocó de baleia!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: ou ainda pior... PÃO BRANCO
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: Vamos ter uma overdose de tanta heroína e pão branco que eles não vão conseguir pôr o nosso corpo gordo na fornalha do crematório!
{{/if}}

{{if !_.whitebread}}
b: Vamos ter uma overdose de tantas drogas que o agente funerário se vai perguntar como é que o nosso corpo *já* foi pré-embalsamado!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: Além disso, não podemos festejar, precisamos de trabalhar ou seremos um terrível parasita da sociedade!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: DEUS. Se isso te fizer calar a boca, tudo bem.

h: Vou dizer não.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Tudo o que fazemos é chorar num canto sobre como a solidão é tão mortal quanto 15 cigarros por dia.
{{/if}}

{{if _.parasite}}
b: Tudo o que fazemos nas festas é preocupar-nos sobre como deveríamos ser produtivos.
{{/if}}

{{if _.whitebread}}
b: Tudo o que fazemos é preocupar-nos sobre como as opções de alimentos pouco saudáveis nos vão matar.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: credo, pergunto-me porquê.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Então, se formos, vão sentir-se mal, mas, se rejeitarmos o convite, também se vão sentir mal!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: TUDO O QUE FAZEMOS É FAZER COM QUE AS PESSOAS SE SINTAM MAL

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Ugh. Se isso te fizer calar a boca, tudo bem.

h: Vou ignorar o convite.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: Enfim. O Facebook é demasiado. Preciso de algo mais calmo, que gere menos ansiedade.

`hong({eyes:"neutral"});`

h: O que há de novo no Twitter?

`bb({eyes:"look"});`

[Oh não, olha para esta notícia horrível!](#act1d_news)

[Oh não, este tweet é secretamente sobre *nós?*](#act1d_subtweet)

[Ei, um GIF de um gato a beber leite](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Deus, parece que o mundo está a arder, não é?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Parece que está tudo a acabar, como se tudo estivesse a morrer e estivéssemos condenados e não há nada que possamos fazer sobre isso.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Vamos dar retweet a esta história!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Ok, vou dar retweet, mas por favor, fica quieto!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: Que se ^foda^, vamos dar uma vista de olhos ao Snapchat.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: É um subtweet! Um subtweet muito sorrateiro!

`hong({eyes:"annoyed"});`

h: Provavelmente não.

`bb({eyes:"narrow", mouth:"small"});`

b: mas e se eles estiverem a falar pelas nossas costas

h: Não est--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: EM FRENTE ÀS NOSSAS COSTAS

`hong({eyes:"sad", mouth:"sad"});`

h: Eu n-

`bb({eyes:"narrow", mouth:"small"});`

b: mas *e se*

h: P--

`bb({eyes:"narrow_eyebrow"});`

b: *e se*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: OK, vou tentar o Snapchat.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Heh ya que fofo, acabei de dar retweet, ach--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: OS GATOS NÃO CONSEGUEM DIGERIR O LEITE E SOMOS HORRÍVEIS POR APRECIAR ABUSO ANIMAL

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: OK, vou tentar o Snapchat.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Huh, fotos de ontem à noite. Então é *assim* que são aquelas festas semanais.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Oof, parece demasiada gente para a minha ansiedade.

h: Talvez eu não devesse ter dito sim ao convite?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Mudar a nossa resposta? Como um idiota?!](#act1e_yes_dontchange)

[Muda a nossa resposta! É demasiada gente!](#act1e_yes_changetono)

{{if _.subtweet}}
[Sim, eles estavam a subtweetar-nos de certeza.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Espera, demos retweet sem verificar os factos.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet &&!_.badnews)}}
[Sabes que tens uma postura muito má?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Eles estavam a contar com a nossa presença e agora traímos a confiança deles? Queres morrer sozinho?!

{{if _.fifteencigs}}
b: QUINZE. CIGARROS.
{{/if}}

{{if _.whalepoop}}
b: COCÓ. DE BALEIA.
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Cala-te, cala-te, vou manter a resposta como um sim!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Não sabes o que é uma debandada humana?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Em 2003, um bar em Rhode Island teve um incêndio e o pânico fez com que as pessoas congestionassem as saídas, então 100 pessoas morreram queimadas-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: QUERES QUE ISSO ACONTEÇA CONNOSCO-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: DIZ NÃO DIZ NÃO DIZ NÃO DIZ NÃO DIZ NÃO DIZ NÃO DIZ NÃO DIZ NÃO DIZ N-


```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Cala-te, cala-te, vou mudar a minha resposta para não! Deus!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... parece muito divertido.

h: Talvez eu não devesse ter dito não ao convite?

`bb({mouth:"normal", eyes:"normal"});`

[Mudar a nossa resposta? Como um idiota?!](#act1e_no_dontchange)

[Muda a nossa resposta! Não morras sozinho!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Sim, eles estavam a subtweetar-nos de certeza.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Espera, demos retweet sem verificar os factos.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Sabes que tens uma postura muito má?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Estava toda a gente a contar connosco!

b: ...para deixá-los em paz e deixá-los ter uma boa festa sem um horrível e asqueroso {{if _.whitebread}}verme mastigador de pão{{/if}} branco como n--


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Cala-te, cala-te, vou manter a resposta como um não!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: A solidão crónica aumenta os nossos níveis de cortisol, bem como o risco de doenças cardiovasculares e derrames!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: QUINZE. CIGARROS.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Cala-te, cala-te, vou mudar a minha resposta para sim! Deus!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Todos os nossos tweets problemáticos voltaram ao de cima!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: Vamos estar na boca de toda a gente, vamos ser cancelados e arrastados com uma corda pela autoestrada da informação!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Porque é que és assim?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Estamos a espalhar desinformação! Estamos a destruir a confiança na imprensa livre!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Nós somos a razão pela qual o fascismo renascerá dos escombros da democracia!

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: Porque é que és assim?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Queres que a tua coluna seja um pretzel?! Para de te curvares sobre o ecrã!

```
bb({body:"meta"});
```

b: Isto também se aplica a ti.

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Porque é que és assim?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... parece muito divertido.

h: Talvez eu não devesse ter ignorado o convite?

`bb({mouth:"normal", eyes:"normal"});`

[Continue a ignorar, ainda somos desmancha-prazeres.](#act1e_ignore_continue)

[Na verdade, diz sim.](#act1e_ignore_changetoyes)

[Na verdade, diz não.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: É meio rude continuar a ignorá-los, não?

`bb({eyes:"normal_right"});`

b: Bem, as pessoas também estão sempre a ignorar-*nos*, por isso...

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: vamos só ficar quites.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: Estás a deixar que me... divirta?

b: Bem, a solidão *pode* matar-nos.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: Tem demasiada gente. Multidões são perigosas.

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Tanto faz. Nova notificação do Tinder.

`bb({eyes:"uncertain"})`

b: O quê, aquela app para curtes?

`hong({eyes:"annoyed"})`

h: Não é uma app para curtes, é só uma maneira de conhecer pesso--

`bb({eyes:"narrow"})`

b: É uma app para curtes.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: Oh, tive um match! Parece giro!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Por favor, não estragues--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: PERIGO PERIGO PERIGO PERIGO PERIGO PERIGO

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Estamos a ser *usados* por outras pessoas.](#act1f_used_by_others)

[Estamos a *usar* outras pessoas.](#act1f_using_others)

[O TEU MATCH É UM ASSASSINO EM SÉRIE](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Conexões aleatórias podem preencher o buraco lá em baixo,

b: mas eles nunca podem preencher o buraco...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: *aqui*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: A questão é que NÓS VAMOS MORRER SOZINHOS

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: Achas que os órgãos genitais das outras pessoas são como Pokémons para colecionarmos?

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ (música tema do Pokémon)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ Eu quero ser a mais ^put^ona-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ Como nunca ninguém foi-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ Coxas e ^cu^, mamas voluptuosas-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ com um ^pénis^ e bolas suadas!-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ TARADO-MON! VOU APANH-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: A questão é que somos um idiota manipulador.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: Vão prender-te num poço e forçar-te a comer pão branco para te engordar para que possam vestir a tua pele como um fato!
{{/if}}

{{if _.parasite}}
b: Eles vão espancar-te com um cronômetro e dizer "TENS DE SER MAIS PRODUTIVO Ó PARASITA"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Eles vão transformar a tua carne em confettis e transformar as tuas entranhas em serpentinas e misturar o teu sangue numa tigela de ponche!
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: O que achas disso como um convite para uma festa?!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: estou tão farto deste jogo.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"a solidão vai-nos matar"... {{/if}}
{{if _.parasite}}"somos um parasita da sociedade"... {{/if}}
{{if _.whitebread}}"não comas isso, vai-nos matar"... {{/if}}
{{if _.subtweet}}"eles estão a falar nas nossas costas"... {{/if}}
{{if _.badnews}}"o mundo está a arder"... {{/if}}
{{if _.hookuphole}}"vamos morrer sozinhos"... {{/if}}
{{if _.serialkiller}}ele é um assassino em série"... {{/if}}
{{if _.catmilk}}"gatos não conseguem digerir leite"... {{/if}}
{{if _.pokemon}}uma canção paródia de ^merda^... {{/if}}

h: eu só quero viver a minha vida.

h: eu só me quero livrar de toda esta... dor.

`bb({eyes:"look_sad"});`

b: Ei... humano...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: Vai ficar tudo bem.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: Como o teu fiel Lobo de Guarda, vou ficar sempre de olho no perigo e vou manter-te seguro.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: Eu prometo.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Última app. Instagram. O que tem de bom?

`hong({eyes:"sad"});`

h: São... mais fotos de festas.

`hong({mouth:"sad"});`

h: Toda a gente parece tão feliz. Livre de preocupações. Livre de ansiedade.

`hong({mouth:"anger"});`

h: Deus, porque é que não posso ser como eles? Porque é que não posso ser apenas *normal?*

`bb({eyes:"normal_right"});`

b: Por falar em festas, sobre o convite deste fim-de-semana. Esta é minha decisão FINAL:

`bb({eyes:"normal"});`

[Devemos ir.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[Não devemos ir.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: Nós deve--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: VAI-TE

`hong({body:"2_you"});`

h: *^FODER^.*

(...500)

b: o-

(...1500)

`bb({eyes:"wat_2"});`

b: o qu-?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: Eu vou dizer SIM à festa,

{{if _.act1g=="go"}}
h: NÃO porque tu queres, mas porque *eu* quero.
{{/if}}

{{if _.act1g=="dont"}}
h: Precisamente PORQUE tu não queres que eu diga sim.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: Tu NÃO me controlas.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: Agora, com licença, enquanto eu como esta deliciosa sandes em paz.

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[AHHHH NÓS VAMOS MORRER](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH TODOS NOS ODEIAM](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH SOMOS PESSOAS HORRÍVEIS](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH NÓS VAMOS MORRER AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH TODOS NOS ODEIAM AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH SOMOS PESSOAS HORRÍVEIS AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: PARABÉNS

(...500)

n: PROTEGESTE COM SUCESSO AS NECESSIDADES FÍSICAS + SOCIAIS + MORAIS DO TEU HUMANO

n: OLHA COMO ESTÁ GRATO!

(...500)

n: AGORA QUE A ENERGIA DELE ESTÁ NO ZERO, PODES CONTROLAR DIRETAMENTE AS SUAS AÇÕES

`bb({mouth:"smile", eyes:"normal"});`

n: ESCOLHE A TUA JOGADA FINAL

`bb({mouth:"small_lock", eyes:"fear"});`

n: *ACABA COM ELE*

[{LUTA: Pune o teu telemóvel stessante!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{FOGE: Enrola-te numa bola e chora!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: O teu telefone estava a causar-te um ataque de pânico!

`bb({eyes:"anger"})`

b: O Zuckerberg e companhia estão a sequestrar a tua saúde mental por dinheiro!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Castiga o teu telemóvel! Destrói-o! Mata-o!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: MATA-O, MATA-O, MATA-O, MATA-O, MATA-O, MATA-O, MATA-O, MATA-O, MATA-O, MATA-O, MATA-O, MATA-O, MAT--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: O mundo inteiro está cheio de perigo!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Faz como o tatu! Enrola-te numa bola para autodefesa!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: ENROLA-TE E CHORA ENROLA-TE E CHORA ENROLA-TE E CHORA ENROLA-TE E CHORA ENROLA-TE E CH--

(#act1j)

# act1j

`SceneSetup.act1_outro()`