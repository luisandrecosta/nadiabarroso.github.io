# act4

```
SceneSetup.act4();
publish("SAVE_GAME", ["act4"]);
Game.FORCE_CANT_SKIP = true;
```

(...5001)

```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n3: (game auto-saved)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
var hong_frame = _.INJURED ? 9 : 0;
publish("act4", ["hong_walks_in",hong_frame]);
sfx("grass_step1", {volume:0.1});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.2});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.25});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.3});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...1667)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...1333)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.20});
```

(...167)

```
publish("act4_hong_sits");
```

(...66)

```
publish("act4", ["hong_transition", "next"]);
sfx("squeak");
```

(...133)

`publish("act4", ["hong_transition", "next"]);`

(...1333)

```
publish("act4", ["hong_transition", "next"]);
sfx("rustle");
```

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1001)

```
publish("act4", ["hong_transition", "next"]);
```

(...333)

```
publish("act4", ["hong_transition", 9]);
sfx("sandwich");
```

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1466)

`publish("act4-out-1");`

(...201)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

```
publish("act4-show-chars");
Game.FORCE_CANT_SKIP = false;
```

(...901)

`hong({body:"sigh_1"})`

(...601)

```
hong({body:"sigh_2"});
bb({eyes:"look_down"});
```

h: *suspiro*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Então, que ^caralho^ foi a moral desta história?

`hong({body:"one_up", eyes:"annoyed"})`

h: O que é que *aprendemos*? Eu *estava* a ser estúpido, os meus "amigos" *estavam* a usar-me, e nós quase *morremos*.

`hong({body:"normal", eyes:"normal"})`

{{if _.harm}}
[Sim, sem mencionar a conta do hospital.](#act4a_bill)
{{/if}}

{{if !_.harm}}
[Sim, sem mencionar os danos ao fígado.](#act4a_liver)
{{/if}}

[Sim, esse *era* o pior cenário possível.](#act4a_worst)

[Sim, eu tinha razão.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: Certo. Eu não acho que o meu seguro cobre "ser estúpido".

`hong({eyes:"annoyed", mouth:"normal"});`

b: E ainda assim... sobrevivemos!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: Tenho a certeza de que reduzimos alguns anos à nossa vida...

`bb({eyes:"surprise"});`

b: Mas pelo menos ainda *temos* vida! Nós sobrevivemos!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: E ainda assim...

h: Hm?

`bb({eyes:"surprise"});`

b: Nós sobrevivemos!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: Mas... também tinhas razão.

`hong({eyes:"surprise"});`

h: Hm?

`bb({eyes:"normal"});`

b: Eu *fui* o lobo que gritou lobo. Então quando me deparei com perigo *real*, tu - e com razão - não acreditaste em mim.

`bb({eyes:"surprise_r"});`

b: E ainda assim... sobrevivemos!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: Apesar de tudo, ainda aqui estamos.

`hong({eyes:"suspect"});`

{{if _.harm}}
h: Pareces bastante calmo, considerando que acabamos de ter uma experiência de vida ou morte.
{{/if}}

{{if !_.harm}}
h: Pareces bastante calmo, considerando que acabamos de ter uma experiência de vida *ou* morte.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: Bem, comparado a isso, tudo o resto parece menos assustador. Também me fez pensar.

`bb({eyes:"normal", mouth:"normal"});`

b: Se o facto de eu lutar contigo é uma ^merda^, porque não te protege...

h: Mas lutar contigo *também* é uma ^merda^, porque só te faz gritar mais alto...

`bb({eyes:"normal_r"})`

b: Então talvez...

`bb({eyes:"normal"})`

h: Talvez não seja necessário lutarmos.

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
```

(...301)

`publish("smash",[0]);`

(...2001)

```
publish("smash",[1]);
sfx("smash_glass");
```

(...2601)

```
publish("smash",[2]);
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

(...2001)

`Game.FORCE_CANT_SKIP = false;`

(#act4b_2)

# act4b_2

```
music('dontfight',{fade:5, volume:0.6});
bb({eyes:"annoyed_d"});
```

b: Eu não sou um Lobo Mau. Mas também não sou um Lobo de Guarda.

`bb({eyes:"sad_d"})`

b: Eu sou um cão de canil maltratado.

`bb({eyes:"sad"})`

b: Nós passamos por coisas difíceis. Talvez trauma ou negligência. É por isso que por vezes reajo exageradamente e penso:

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: AU AU AU AU AU AU AU AU AU 

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: Mas eu não *quero* ser um Cão Cobarde! Eu quero proteger-te! Eu quero ser um Bom Cão!

`bb({eyes:"sad", mouth:"normal"});`

b: Humano... Podes ajudar-me a domar este Lobo?

`hong({eyes:"sad"})`

h: Eu... Vou tentar.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: Ok. Um relacionamento saudável com emoções. Relacionamentos precisam de comunicação. Então, vamos comunicar.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: Os próximos cinco minutos vão parecer super melosos, mas é como dizem "prática leva à perfeição".

```
hong({body:"hands_2", mouth:"normal"});
```

h: Querido Lobo interior ... como *estás* a sentir-te?

n2: NÚMERO TOTAL DE MEDOS USADOS:

n2: *MAGOADO* {{_.attack_harm_total}}, *NÃO AMADO* {{_.attack_alone_total}}, *MÁ PESSOA* {{_.attack_bad_total}}

n2: DE QUE MEDO QUERES FALAR PRIMEIRO? (PODES FALAR DOS OUTROS MAIS TARDE)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[Estou com medo de sermos magoados.](#act4_harm)

[Estou com medo de ficarmos sozinhos.](#act4_alone)

[Estou com medo de que sejamos más pessoas.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: Eu quero proteger a tua necessidade de segurança física,

`bb({eyes:"sad_d"})`

b: Mas o *mundo* parece tão perigoso. Tão cheio de tragédia e maldade.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: Não sei, chega de ser *eu* a escolher o que dizer a seguir. O que *dizes* , humano?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Outra vez, de volta a ti, humano. O que achas?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Mais pensamentos, humano?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Tens razão. Então, vamos proteger-nos.](#act4_harm_skills)

[Vamos expor-nos a *mais* perigos.](#act4_harm_exposure)

[Obrigado.](#act4_thanks) `_.thanks_for = "physical safety";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Mas ... como? Tenho presas e garras, mas sou apenas uma metáfora.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Podemos aprender autodefesa? Juntarmo-nos a uma comunidade onde nos protegemos uns aos outros? Melhorar a nossa saúde geral e limites pessoais?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: Talvez, mas ...

[Por onde começamos?](#act4_harm_skills_start)

[E se ainda não funcionarem?](#act4_harm_skills_work)

[E se exagerarmos na "segurança"?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: Há tanto a fazer, tanta coisa que precisamos de consertar em nós mesmos. Com o que *começamos*?

`hong({ body:"shrug", eyes:"surprise" })`

h: Estamos a começar agora.

`bb({ eyes:"normal", mouth:"narrow" })`

b: Ah?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: Estamos a praticar boa comunicação agora. O que nos ajudará a detetar melhor o perigo, com menos falsos positivos,

`hong({ eyes:"surprise" });`

h: E *isso* vai ajudar-nos a proteger contra o perigo!

`hong({ eyes:"normal", mouth:"normal" });`

h: Portanto: isto *é um* treino de autodefesa.

`bb({ eyes:"normal_r" })`

b: Huh. Eu estava à espera de algo como:

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
hong({ eyes:"sad", mouth:"smile" });
bb({ body:"karate_1" });
sfx("hiya");
```

(...1001)

`Game.FORCE_CANT_SKIP = false;`

(#act4_something_else)

# act4_harm_skills_work

`bb({ eyes:"normal" });`

h: Verdade, não há como nos proteger a 100%...

`hong({ body:"one_up" });`

h: Mas mesmo uma melhoria de 1% já vale alguma coisa, certo?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: Estás a ver o copo, não como 99% vazio, mas como 1% cheio?

`bb({ eyes:"normal" });`

h: O que ainda vale alguma coisa se estiveres perdido no deserto.

`bb({ eyes:"closed" });`

b: Bem. Bota abaixo, então.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: Quer dizer, tu só ignoraste os meus avisos porque *eu exagerei* com a segurança!

`bb({ body:"normal", eyes:"normal" })`

h: Não, tens razão. Segurança em moderação. Tudo em moderação.

`bb({ eyes:"suspect" })`

b: Desculpa, *TUDO* em moderação?

`hong({ eyes:"annoyed" })`

h: *Um número moderado de coisas* em moderação.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Obrigada por fazeres as tuas declarações recursivamente auto consistentes.

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *O QUÊ*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: Quer dizer, digamos que um Cão tem medo da trovoada.

`hong({ body:"hands_1" });`

h: Um truque que os treinadores usam é tocar uma gravação de trovoada num volume baixo e, a seguir, dão ao cão uma recompensa por ficar calmo.

`hong({ body:"hands_2" });`

h: Ao longo de vários dias, o treinador aumenta o volume aos poucos, até que o Cão supere o medo de trovões.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: Chama-se terapia de exposição!

`hong({ body:"point", eyes:"normal" });`

h: Já que és um Cão, deve funcionar para ti também, certo? Todos os mamíferos têm a mesma resposta no que toca a "luta ou fuga".

`hong({ body:"normal" });`

[E se dessensibilizarmos *demais*?](#act4_harm_exposure_overboard)

[E se estivermos expostos a um perigo *real*?](#act4_harm_exposure_hurt)

[Eu sou um Lobo, não um Cão.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: Eu vou mostrar-te bondade e paciência até estares domesticado e virares um cãozinho fofinho.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: Duh.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: *Acabamos* de ver o que acontece se bloqueares o teu medo - pões-te em situações *realmente* perigosas.

`bb({ eyes:"angry_r", body:"one_up" })`

b: Além disso, *demasiada* dessensibilização não nos vai transformar em psicopatas?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: Daqui a bocado, vamos estar a recompensar-nos enquanto vemos pornografia de "snuff"!

`hong({ eyes:"annoyed" })`

h: Eu... acho que há uma linha entre isso e a trovoada.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: Mas *onde* exatamente, humano? *Onde?!*

`hong({ eyes:"surprise", body:"one_up" })`

h: Não sei. Mas *podes* ajudar-me!

`hong({ eyes:"normal", body:"normal" })`

h: Ao trabalhar e negociar contigo, conseguiremos traçar essa linha.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: Ok. Mas eu não tenho polegares, por isso vais ter de ser tu a desenhar.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.harm}}
b: Por exemplo: saltamos de um *telhado!*
{{/if}}

{{if !_.harm}}
b: Por exemplo: quase saltamos de um *telhado!*
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: Nah, tens razão. *Podemos* ir mais longe.

`hong({ eyes:"normal" });`

h: Mas é por isso que, se fizermos terapia de exposição, começaremos devagar e daremos pequenos passos para melhorar.

h: Antes de atingirmos o perigo *real*, paramos.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Sim, eu traço a linha entre ouvir um trovão alto e ficar no meio de uma tempestade com um chapéu alto e pontiagudo.

(#act4_something_else)

# act4_thanks

`_.num_thanks += 1`

{{if _.num_thanks==1}}
(#act4_thanks_1)
{{/if}}

{{if _.num_thanks==2}}
(#act4_thanks_2)
{{/if}}

{{if _.num_thanks==3}}
(#act4_thanks_3)
{{/if}}

# act4_thanks_1

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"annoyed" })`

b: Espera, nenhum argumento a favor ou contra o que estou a sentir? Só... "obrigado"?

`hong({ eyes:"surprise", body:"shrug" })`

h: Sim! Obrigado por mostrares a tua preocupação com as minhas {{_.thanks_for}}.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: Estás bem?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: Nunca *me tinhas* agradecido antes.

`hong({ mouth:"smile" });`

h: Aw, seu grande e felpudo Lobo stressado.

(#act4_something_else)

# act4_thanks_2

h: Mesmo que reajas de forma exagerada, agradeço por cuidares do meu {{_.thanks_for}}.

`bb({ eyes:"annoyed" })`

b: Espera... não estás só a repetir "obrigado" para evitar realmente falar sobre esses medos, ou estás?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Bem, as coisas são complicadas e nem sempre tenho as respostas prontas.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: Não é como se a vida nos desse uma lista de 3 respostas de diálogo predefinidas.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: Mas, por agora, posso pelo menos dizer obrigado.

b: Bem, obrigado também por me ouvires tão pacientemente.

`bb({ eyes:"closed" });`

b: Seu pequeno e careca mamífero.

(#act4_something_else)

# act4_thanks_3

h: Mesmo que os teus latidos me assustem, sei que estás apenas a tentar proteger-me {{_.thanks_for}}.

`bb({ eyes:"smile_r" });`

b: Ok, se continuares a elogiar-me assim, a internet vai ficar com algumas ideias estranhas sobre nós.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: Por amor de Deus, sou apenas um bebé universitário vulnerável e tu és um Lobo grande e assustador. O que é o pior que pod-

`hong({ eyes:"normal", body:"point" });`

h: Na verdade, não respondas a isso.

(#act4_something_else)



# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: Eu quero ter a certeza de que preenches a tua necessidade de pertencer...

`bb({ eyes:"sad_u" });`

b: Mas preocupa-me que, caso alguém nos conheça - o *verdadeiro* nós - se assustem connosco.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: Não sei, chega de ser *eu* a escolher o que dizer a seguir. O que *dizes* , humano?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Outra vez, de volta a ti, humano. O que achas?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Mais pensamentos, humano?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Concordo: vamos trabalhar na nossa vida social.](#act4_alone_skills)

[Acho que as pessoas gostam de nós. Vamos descobrir?](#act4_alone_experiment)

[Obrigado.](#act4_thanks) `_.thanks_for = "social belonging";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: Poderíamos praticar habilidades como fazer perguntas, ouvir e ter empatia, ser aberto e vulnerável, etc?

`hong({ eyes:"normal_l" });`

h: Ou criar hábitos sociais melhores, como planear qualquer coisa com amigos ou sair regularmente?

`hong({ body:"one_up" });`

h: Também poderíamos aprender a ficar mais confortáveis com rejeição.

`hong({ eyes:"normal" });`

h: Ou aprender a saber quando as pessoas *não* nos estão a rejeitar, estão apenas cansadas ou têm Resting ^Bitch^ Face.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: Há muitas opções. Mas, sobre "aprender habilidades sociais"...

[Isso não é *manipulador?*](#act4_alone_skills_manipulative)

[Não nos tornará *mais fáceis de manipular?*](#act4_alone_skills_manipulated)

[E se falharmos?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: Os serial killers que podem ler as emoções das vítimas não são ótimos com "empatia"?

`bb({ eyes:"annoyed" });`

b: O Charles Manson não arranjou amigos e influenciou pessoas?

`hong({ eyes:"annoyed", body:"chin" });`

h: Não, tens razão.

h: "Habilidades sociais" não significam nada se não quisermos, genuinamente, saber *das* pessoas.

`hong({ body:"normal" });`

h: Basicamente, basta não ser ^imbecil^.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: Está aí uma magnifica frase para um póster motivacional.

`hong({ body:"shrug", mouth:"narrow" });`

h: “Não sejas ^Imbecil^ ™”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: Vamos tornar-nos tapetes de boas-vindas, a dizer "por favor" e "obrigado" enquanto as pessoas limpam os pés em nós!

`bb({ mouth:"scream", eyes:"scream" })`

b: Vamos lamber tantas botas, vai parecer que estamos usar graxa nos lábios!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: Não, tens razão. "Habilidades sociais" não pode ser apenas para agradar aos outros, também serve para estabelecer *limites.*

`hong( body:"one_up" });`

h: Não podemos convidar outras pessoas para a nossa casa, se não tivermos paredes para sustentá-la.

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: Já agora...: aquela imagem mental dos lábios... *ew??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: Podemos falhar. Na verdade, *iremos* falhar.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: Mas não há problema! Fracassar é como se aprende!

`hong({ body:"normal", eyes:"normal" });`

h: Então, vamos avançar juntos, ok?

`bb({ eyes:"normal_r" });`

b: Claro, acho... na pior das hipóteses, podemos simplesmente fugir da cidade e arranjar uma identidade nova.

`bb({ eyes:"normal" });`

h: Sim, acho que isso só custa duas bitcoins hoje em dia.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Podíamos fazer algumas experências!

`hong({ body:"chin" });`

h: Podíamos enviar um ping a um amigo para sair, reconectar com um colega ou até conversar com o barista.

`hong({ body:"normal" });`

h: Acho que vamos descobrir que somos mais simpáticos do que pensamos.

`bb({ eyes:"annoyed" });`

[E se essas forem "vitórias" pequenas?](#act4_alone_experiment_cheap)

[E se isso for inconveniente para os outros?](#act4_alone_experiment_burden)

[Mas conversa fiada não é o "*verdadeiro* nós"!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Se pusermos um sorriso falso, nunca vamos realmente conectar-nos com ninguém,

`bb({ eyes:"super_sad" });`

b: *Mas* se nos abrirmos, as outras pessoas irão ver as nossas entranhas!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Rebola.

b: O quê.

`hong({body:"hands_1"})`

h: Quando os cães querem mostrar amor e confiança, eles tornam-se vulneráveis ao expôr a barriga.

`hong({body:"one_up"})`

h: Talvez *ainda* não estejamos seguros o suficiente para sermos muito vulneráveis, mas com treino suficiente,

`hong({body:"normal", eyes:"surprise"})`

h: Um dia podemos mostrar às pessoas quem somos na realidade - todos confusos, todos humanos.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Vou rebolar se me deres mimos.

`bb({ eyes:"normal", mouth:"normal" });`

h: Não.

(#act4_something_else)


# act4_alone_experiment_cheap

b: Dizer "Olá" ao barista não é exatamente o desempenho de medalha de ouro nas Olimpíadas das Borboletas Sociais.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Para *nós é!*

`hong({ body:"one_up", eyes:"annoyed" });`

h: Na área social, nem do escalão dos "featherweight" somos, somos como... "quark-weight".

`hong({ body:"normal", eyes:"normal" });`

h: Se tivermos de começar com vitórias pequenas, assim seja. Há que subir o primeiro degrau antes do milésimo degrau.

b: Sim! Talvez depois de dizer "Olá", possamos avançar para um...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"Tudo bem?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Sim e contigo!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Talvez o barista só queira fazer o raio do café e não fazer parte de uma *experiência* para ver se nossas habilidades sociais são más.

`bb({ eyes:"annoyed" })`

h: Bem, se for óbvio que *somos* um inconveniente...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: É bom que o saibamos também!

`hong({ eyes:"normal" });`

h: Mais tarde podemos aprender a perguntar proativamente às pessoas aquilo com que se sentem confortáveis, para saber e respeitar os limites delas.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Tu sabes, aquela ^merda^ de "habilidades interpessoais" que vemos nos panfletos.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Eu quero defender as tuas necessidades morais, essa vontade de ter tornares uma pessoa melhor,

`bb({ eyes:"sad_d" })`

b: Mas parece que, no fundo, estamos fundamentalmente... despedaçados.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.harm}}
b: E não me digas que *não* estamos confusos. Saltamos de um *telhado*.
{{/if}}

{{if !_.harm}}
b: E não me digas que *não* estamos confusos. Quase saltamos de um *telhado*.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: Não sei, chega de ser *eu* a escolher o que dizer a seguir. O que *dizes* , humano?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Outra vez, de volta a ti, humano. O que achas?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Mais pensamentos, humano?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Então estamos despedaçados. Vamos consertar-nos.](#act4_bad_fix)

[Então estamos despedaçados. Vamos aceitar isso.](#act4_bad_accept)

[Obrigado.](#act4_thanks) `_.thanks_for = "moral well-being";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Podemos ir construindo hábitos melhores, colocar a nossa vida mais alinhada com o que valorizamos,

`hong({body:"one_up"});`

h: E se for necessário, podemos arranjar ajuda profissional - um terapeuta ou conselheiro.

`hong({body:"normal"});`

h: Existem maneiras de nos consertar.

[E se não conseguirmos consertar tudo?](#act4_bad_fix_cant)

[E se consertarmos em *demasia*?](#act4_bad_fix_too_much)

[Não podemos pagar ajuda profissional.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Não, acho que tens razão.

h: Não podemos consertar tudo.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: Ahhh eu sabia que ficaríamos despedaçados para sempre!

`hong({eyes:"surprise"});`

h: Mas podemos, pelo menos, ser "não *tão* " despedaçados.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: As cicatrizes curam com o tempo, mas nunca desaparecem. E não há problema.

`bb({eyes:"annoyed_r"});`

b: Talvez. Além disso,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: Cicatrizes são *sexy.*

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: Por favor, não faças isso.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: É doentio admitir, mas... parte de mim *quer* ter este transtorno.

`bb({ eyes:"angry" })`

b: Quer dizer, sem ele, não seríamos *aborrecidos?*

`bb({ eyes:"sad_r", body:"one_up" })`

b: Sem a desordem, a nossa arte não se tornaria obsoleta e sem graça?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Sem o transtorno, não seríamos incapazes de nos conectar com os nossos amigos que têm o transtorno?

`bb({ eyes:"sad", body:"chest" })`

b: Se estivermos sempre contentes com a vida, não vamos parar de nos esforçar para fazer coisas extraordinárias?

`hong({ MOUTH_LOCK:true })`

h: ...

h: Se tivermos medo de ... "esgotar os nossos medos" ...

h: Eu não acho que vamos ficar sem medos.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Oh, sim! Ufa! Que alivio!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "Doutor, estou ansioso por pagar 100€ à hora só para o ouvir perguntar "*Como é que isso te faz sentir"?*"

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "Mm-hmm. E como é que isso te faz sentir?

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Nah, essa é uma preocupação totalmente razoável.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: E é realmente uma pena que a saúde mental não seja acessível para muitas pessoas.

`hong({ eyes:"normal", mouth:"normal" });`

h: Ainda assim, existem algumas opções baratas ou gratuitas:

`hong({ body:"chin" })`

h: Grupos de apoio, terapia online, centros de saúde estudantis / sem fins lucrativos...

`hong({ body:"hands_1" })`

h: Construir hábitos como meditação, dormir bem, conversar regularmente com amigos, aprender coisas novas ...

`hong({ body:"hands_2" })`

h: Ir à biblioteca buscar livros de exercícios para psicoterapias baseadas em evidências ...

`hong({ body:"one_up" })`

h: Há uma lista completa de recursos no final deste jogo!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Bem, *esta* "fourth wall" não durou muito.

`hong({ body:"point" });`

h: Algumas coisas são mais importantes do que a convenção narrativa. Como a saúde mental.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: Quer dizer, é isso que dizem os terapeutas, certo? Aceita todas as tuas emoções, mesmo as negativas?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Espera.

["Aceitar" como em *desistir*?](#act4_bad_accept_give_up)

["Aceitar" como em *aprová-las*?](#act4_bad_accept_approve)

["Aceitar" como em levá-las *a sério*?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Achas que o Martin Luther King teria dito: "É uma ^merda^ não nos podermos sentar na parte da frente do autocarro, mas vamos só *aceitar* ?"

`bb({ eyes:"angry_r", body:"two_up" });`

b: Por que é que o Complexo Industrial de Autoajuda acha que acenar a bandeira branca é *sabedoria profunda?*

`bb({ eyes:"annoyed", body:"normal" });`

h: Eu acho que os terapeutas querem dizer "aceitar" coisas más como em: reconhecer que existem e são difíceis de mudar,

h: Mas não necessariamente desistir de um compromisso com a mudança.

`bb({ eyes:"suspect" });`

b: Então os terapeutas devem dizer *reconhecer*, não *aceitar*.

`hong({ body:"chin", eyes:"annoyed" });`

h: Sim, pensando bem, "aceitar" é meio confuso.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Bem, eu *reconheço* isso.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Como é *bom* estarmos despedaçados ou algo assim? Não!

`bb({ eyes:"angry_r", body:"one_up" });`

b: Todos aqueles argumentistas de Hollywood que romantizam doenças mentais estão cheios de ^merda^ na cabeça!

`bb({ eyes:"angry", body:"two_up" });`

b: Ter um transtorno mental é uma ^*merda^!* Rouba *vida às pessoas!* Porque é que devemos "aceitar" isso?!

`bb({ body:"normal" });`

h: Acho que terapeutas querem dizer "aceitar" as nossas emoções como em: sejam pacientes com elas.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Por exemplo, da mesma maneira que nos mexermos em areia movediça nos faz afundar mais rápido, e a solução é ficar pacientemente quieto,

`hong({ eyes:"surprise" });`

{{if _.harm}}
h: Lutar contra ti, o meu medo, levou-me a saltar de um telhado.
{{/if}}

{{if !_.harm}}
h: Lutar contra ti, o meu medo, quase me levou a saltar de um telhado.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: Em vez disso, a solução é fazer o que estamos a fazer agora - não lutar, mas estar pacificamente um com o outro.

`bb({ eyes:"annoyed" });`

b: Então eles deviam dizer *isso* em vez de uma palavra tão problemática como "aceitar".

`hong({ body:"chin", eyes:"annoyed" });`

h: Sim, pensando bem, "aceitar" é uma ^merda^.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: Não aceito "aceitar".

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: Mas já *sabemos* que não deves levar-me a sério!

`bb({ eyes:"sad_u", body:"two_up" });`

b: O *problema* é que eu quero ajudar-te, mas sou péssimo a usar palavras para fazer isso!

`bb({ eyes:"sad", body:"normal" });`

h: Acho que os terapeutas querem dizer "aceitar" as emoções como em: "não lutes com elas nem as ignores".

`hong({ eyes:"surprise", body:"one_up" });`

h: Para te ouvir, trabalhar *contigo* , mas não tomar o que dizes como uma verdade 100% literal.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: Então os terapeutas deviam dizer *isso* em vez de uma palavra tão confusa e vaga como "aceitar".

`hong({ body:"chin", eyes:"annoyed" });`

h: Eu acho que eles são péssimos no que toca ao uso de palavras.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Enfim, queres falar de mais alguma coisa?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: Então, há mais alguma coisa a pesar nesse teu coração?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[Estou com medo de sermos magoados.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[Estou com medo de ficarmos sozinhos.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[Estou com medo de que sejamos más pessoas.](#act4_bad)
{{/if}}

[Nah, estou bem por agora.](#act4c_prelude)

# act4_something_else_2

h: Ok, acho que já falamos sobre todos os nossos medos.

b: Sim, existem apenas três medos.

h: Sim, exatamente, três.

b: Conveniente.

(#act4c)

# act4c_prelude

h: Boa conversa equipa.

(#act4c)

# act4c

```
Game.clearText();
music(null,{fade:3});
bb({body:"normal", eyes:"normal", mouth:"normal", MOUTH_LOCK:true},0);
hong({body:"normal", eyes:"normal", mouth:"normal"},0);
```

b: ...

`hong({MOUTH_LOCK:true},0)`

h: ...

`bb({eyes:"annoyed_d"})`

b: Isto não é um *jogo*, sabes.

`bb({eyes:"angry_d", body:"one_up"})`

b: Construir um relacionamento saudável com as tuas emoções não é tão simples como clicar em botões numa tela.

`bb({eyes:"sad", body:"normal"})`

b: *Podemos* mesmo dar-nos bem?

b: *Podemos* trabalhar juntos, como uma equipa?

`hong({eyes:"sad", body:"one_up"})`

h: Bem,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: C-com licença ...

```
Game.clearText();
publish("act4-in-2");
music('campus', {volume:0.5, fade:1});
```

(...2101)

(#act4d)

# act4d

`Game.WORDS_HEIGHT_BOTTOM = 221;`

`publish("act4", ["alshire", 0]);`

a: I-i-importas-te que me sente contigo para almoçar?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *É este* o teu crush? Por que está sentado sozinho como um psicopata?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: A perguntar ao teu crush se te podes sentar com ele? Tens noção do quão *carente* pareces?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *É este* o teu crush? Interrompemos paz e sossego dele! Somos tão inconvenientes!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: Q-q-quer dizer- es-está tudo bem se não puder, eu só...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Espera, não te vi na festa?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Sim, claro! Vem cá.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Desculpa, preciso de um tempo sozinho agora.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Sim, estavas no sofá! Na primeira festa a que fui...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Onde tive aquele ataque de pânico e dei um soco ao anfitrião.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Onde tive aquele ataque de pânico e fugi a chorar.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Espera, humano, podemos estar a deixá-la desconfortáveis.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, não é a minha intenção deixá-la desconfortável!

`publish("act4", ["hong_to_alshire",4]);`

h2: Estou apenas a relembrar-me de um rosto amigo, só isso.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: AHHHHH EU SABIA! ALERTA: PSICOPATA PERIGOSO EM PÂNICO!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AAHHH A PRIMEIRA IMPRESSÃO QUE FIZEMOS FOI "TESTEMUNHASTE O MEU TRAUMA"! Isso significa que nos odeia!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAHHH FIZEMOS ALGUÉM LEMBRAR-SE DE UM EVENTO TRAUMÁTICO. SÓ A NOSSA PRESENÇA JÁ MAGOA OS OUTROS.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Espera, humano, ela parece desconfortável.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, sem pressão, é claro!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Podes sentar-te aqui se quiseres.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: ESTÁ A SER *DEMASIADO* AMIGÁVEL! IGUALZINHO AO TED BUNDY, O ASSASSINO!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: ESTÁ SÓ A FINGIR SER SIMPÁTICO! NINGUÉM QUER, *REALMENTE* , ESTAR PERTO DE NÓS!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AHHH NÓS FAZEMOS SEMPRE OS OUTROS SENTIREM-SE ESQUISITOS! SOMOS TÃO DESAGRADÁVEIS!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Espera, humano, podemos estar a deixá-la desconfortável.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, não quero ser rude!

`publish("act4", ["hong_to_alshire", 6]);`

h2: Só preciso de algum tempo para processar as minhas emoções. Por favor, não leves isto como uma rejeição pessoal.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: QUE PENSAMENTOS DOENTIOS E TORCIDOS ESTÁ A PROCESSAR?! QUE DESEJOS OBSCUROS PREENCHEM O CORAÇÃO DESTE PSICOPATA?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: FOMOS REJEITADOS! NUNCA SEREMOS AMADOS!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: INTERROMPEMOS O PROCESSAMENTO EMOCIONAL DELE! AGORA ESTÁ TRAUMATIZADO PARA SEMPRE E É TUDO CULPA NOSSA!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: FOGE FOGE FOGE FOGE FOGE FOGE FOGE FOGE FOGE FOGE

```
Game.clearText();
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["alshire", 10]);
sfx("pop");
```

(...1001)

```
publish("act4", ["alshire", 11]);
sfx("alshire_run");
```

(...2601)

```
publish("act4-out-3");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
```

(...1201)

`publish("act4-jumpcut-hong");`

h: Huh. Aquilo foi estranho. Pergunto-me o que estava a passar-lhe pela cabeça.

`publish("act4", ["hong_closer", 2]);`

h: Enfim, o que estavas a dizer?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Uh, esqueci-me? Algo sobre equipas e trabalho?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: Dizem que deves "fazer as pazes" com as tuas emoções, como se as tuas emoções fossem *criminosos*.

`publish("act4", ["bb_closer", 7]);`

b: Mas eu quero ter *mais* do que mera paz! Eu quero que sejamos *aliados!*

`publish("act4", ["bb_closer", 3]);`

b: Eu quero ser um bom Cão de Guarda. Assim como a fome e a sede são alarmes para as tuas necessidades físicas,

`publish("act4", ["bb_closer", 8]);`

b: Eu quero ser o alarme para as tuas necessidades *psicológicas* - as tuas necessidades de segurança, pertencimento, bondade.

`publish("act4", ["bb_closer", 1]);`

b: Mas... Eu sou péssimo no meu trabalho, então preciso que me treines.

`publish("act4", ["bb_closer", 4]);`

b: Não sou "sempre válido", nem "sempre irracional". Estou apenas ... a dar o meu melhor. Então, por favor…

`publish("act4", ["bb_closer", 30]);`

b: Ajuda-me a ajudar-te!

`publish("act4", ["bb_closer", 6]);`

b: Porém, ensinar truques novos a um cão velho *vai* demorar um pouco. Talvez *anos.*

`publish("act4", ["bb_closer", 3]);`

b: E por vezes vou ter uma recaída, vou cair nos meus velhos hábitos.

`publish("act4", ["bb_closer", 2]);`

b: Vou latir a sombras. Vou assustar-te com palavras. Posso até mostrar-te algumas imagens intrusivas de... coisas.

`publish("act4", ["bb_closer", 9]);`

b: Desculpa. Eu sou um cão de canil maltratado. Cães maltratados fazem cocô na tua cama de vez em quando!

`publish("act4", ["bb_closer", 4]);`

b: Mas se fores paciente comigo... e te "sentares" comigo...

`publish("act4", ["bb_closer", 8]);`

b: Talvez possas domar este Lobo.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Cão lindo.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[Humano lindo.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

# act4f-pat-hong

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 13]);
```

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...6501)

`publish("act4", ["bb_closer", 15]);`

(...1001)

(#act4f)

# act4f-pat-bb

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 10]);
```

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...6501)

`publish("act4", ["bb_closer", 12]);`

(...1001)

(#act4f)

# act4f

```
Game.FORCE_CANT_SKIP = false;
publish("act4", ["bb_closer", 16]);
publish("act4", ["hong_closer", 5]);
```

{{if _.fifteencigs}}
b: AAAAA AINDA ESTÁS A COMER SOZINHO! QUINZE CIGARROS AAAAA
{{/if}}

{{if _.parasite}}
b: AAAAA AINDA NÃO FOSTE PRODUTIVO ENQUANTO COMÍAMOS, SOMOS PARASITAS DA SOCIEDADE AAAAA
{{/if}}

{{if _.whitebread}}
b: AAAAA ESTÁS A COMER MAIS PÃO BRANCO AAAAA
{{/if}}

```
publish("act4", ["bb_closer", 18]);
publish("act4", ["hong_closer", 6]);
sfx("yaps", {volume:0.6});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 205;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: AU AU AU AU AU AU AU AU AU 

(#credits)
