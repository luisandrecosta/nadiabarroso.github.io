# act2

`SceneSetup.act2();`

{{if _.badnews && !_.factcheck}}
(#act2-preamble-news1)
{{/if}}

{{if _.badnews && _.factcheck}}
(#act2-preamble-news2)
{{/if}}

{{if _.catmilk}}
(#act2-preamble-cat)
{{/if}}

(#act2-preamble-tinder)


# act2-preamble-news1

```
publish("act2",["dee",3]);
```

s: Mas *viste* aquela "notícia" sobre aquela coisa horrível que aconteceu naquele lugar?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: O-olá...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Deus, odeio as notícias. É tudo sensacionalismo e clickbait.

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: B-bela festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Verdade, mas eles estão só a seguir incentivos. O *verdadeiro* problema são as pessoas que clicam no clickbait.

```
publish("act2",["dee",3]);
```

s: Quem daria um retweet a uma notícia terrível e faria todos os seus amigos sentirem-se mal?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, eu sei, né?

(#act2-preamble-end)


# act2-preamble-news2

```
publish("act2",["dee",3]);
```

s: Mas *viste* aquela "notícia" que se tornou viral?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: O-olá...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Sim, totalmente falso. Quem cairia nisso e daria retweet?

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: B-bela festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: A sério pá. Tipo, hellooo, abram o Google e verifiquem os factos primeiro?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, eu sei, né?

(#act2-preamble-end)


# act2-preamble-cat

```
publish("act2",["dee",3]);
```

s: Como estava a dizer, o Complexo Industrial dos Memes explora os gatos.

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: O-olá...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Elabora lá isso.

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: B-bela festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Bem, eu vi alguém a dar retweet a um GIF de um gato a beber leite ontem.

```
publish("act2",["dee",3]);
```

s: Eles não conseguem digerir essa ^merda^! Quem dao aria retweet a um *abuso animal* assim?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, eu sei, né?

(#act2-preamble-end)


# (#act2-preamble-tinder)

```
publish("act2",["dee",1]);
```

s: Então, ya, nunca me chegou a responder!

```
publish("act2",["dee",0]);
publish("act2",["party_hong","next"]);
```

h2: O-olá...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Mesmo que vocês tenham dado match no Tinder?

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: B-bela festa...

```
publish("act2",["party_hong","next"]);
```

{{if _.serialkiller}}
(#act2-preamble-serialkiller)
{{/if}}

{{if _.hookuphole}}
(#act2-preamble-hookuphole)
{{/if}}

{{if _.pokemon}}
(#act2-preamble-pokemon)
{{/if}}

# act2-preamble-serialkiller

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Sim, sei lá! Mas quê, pensou que eu era um *assassino em série* ou assim? Tão paranoico.

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, eu sei, né?

(#act2-preamble-end)


# act2-preamble-hookuphole

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Sim, sei lá! Talvez pense que engates não servem para preencher o vazio no coração?

s: Para de ser tão puritano! Abre a tua mente, depois abre as tuas pernas!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, eu sei, né?

(#act2-preamble-end)


# act2-preamble-pokemon

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Sim, sei lá! Não era assim nada de extraordinário, mas teria sido um bom match!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Tenho de os ter a todos!™

(#act2-preamble-end)


# act2-preamble-end

```
Game.clearText();
publish("act2-out-1");
music(null, {fade:1});
```

(...3000)

```
music('battle', {volume:0.5});
publish("hp_show");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

n: SEGUNDA RONDA: *LUTA!*

[Oh não, todos nos odeiam!](#act2a_social)

[Estás *interessadx* na ruiva?](#act2a_perv)

[Ei, vamos falar sobre o significado da vida.](#act2a_meaning)

# act2a_social

`bb({eyes:"sad"})`

b: Estamos a deixar todos de mau humor por sermos tão coitadinhos!

`bb({eyes:"shock", body:"two_up"})`

b: Estamos a arruinar as boas vibes! Estamos a cometer um homicídio de vibes em primeiro grau!

`bb({eyes:"normal", body:"normal"})`

b: Humano, temos de bazar antes ** que--

```
_.a2_first_danger = 'social';
_.a2_attack_1 = "alone";
```

(#act2b)

# act2a_perv

`bb({eyes:"suspect"})`

b: É mais atraente que nós, o que significa que mesmo que *olharmos*, então -

`bb({eyes:"shock", body:"two_up"})`

b: SOMOS UNS TARADOS

`bb({body:"normal"})`

b: Nós somos tarados, maus, maus, maus, terríveis, pervertidos

```
_.a2_first_danger = 'perv';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2a_meaning

`bb({body:"one_up", eyes:"normal_r"})`

b: No final de tudo, o que podemos fazer que realmente importe?

`bb({body:"normal", eyes:"sad"})`

b: Contribuir para a humanidade? Todas as grandes obras decompõem o caminho de Ozymandias. Amor? A morte fará sempre parte.

`bb({eyes:"sad_r"})`

b: E quanta morte existe! *Nós* vamos morrer. *Os nossos entes queridos* vão morrer.

`bb({eyes:"shock", body:"two_up"})`

b: ^Caralho^, até a Segunda Lei da Termodinâmica diz que o nosso *universo* vai morrer!

`bb({eyes:"suspect", body:"normal"})`

b: Ah, "a morte faz-nos valorizar a vida"? Isso é como dizer que a escravidão é boa porque nos faz valorizar a liberdade!

`bb({body:"one_up"})`

b: Oh, "precisas de criar o teu próprio significado"? Isso é o que os cultistas e os conspiracionistas fazem!

`bb({eyes:"shock", body:"two_up"})`

b: A vida não tem sentido, a morte não tem sentido, mesmo *o sentido* não tem sentido! O que é uma alma mortal deve faz-

```
_.a2_first_danger = 'meaning';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2b

`bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"suspect"})`

b: Hum... consegues ouvir-me, humano?

`bb({eyes:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"shock", mouth:"small_talk", body:"chest", MOUTH_LOCK:true})`

b: *SUSPIRO*

`bb({mouth:"small_talk"})`

b: TENHO DE AVISAR-TE ACERCA...

[*Mais* do mesmo perigo!](#act2b_louder)

{{if _.a2_first_danger=="social"}}
[Um perigo social *diferente*!](#act2b_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[Um perigo moral *diferente*!](#act2b_different_moral)
{{/if}}

[Estás a ignorar o perigo! Isso é perigoso!](#act2b_ignore)

# act2b_louder

`_.a2_first_choice = "louder"`

{{if _.a2_first_danger=="social"}}
(#act2b_louder_social) {{/if}}

{{if _.a2_first_danger=="perv"}}
(#act2b_louder_perv) {{/if}}

{{if _.a2_first_danger=="meaning"}}
(#act2b_louder_meaning) {{/if}}

# act2b_louder_social

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: AS EMOÇÕES SÃO CONTAGIOSAS! POR ISSO, SE NÃO FORES EMBORA, VAIS CONTAGIAR TODA A GENTE COM A TUA DOENÇA MENTAL!

b: Vais criar um surto mortal de SÍMDROME DE COITADINHO

`bb({eyes:"suspect", body:"normal", mouth:"normal"})`

b: Precisamos de sair daqui e ficar em quarentena para sempre numa sala com Netflix e take-out!

```
_.a2_second_danger = 'netflix';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "a quarantine";
```

(#act2c)

# act2b_louder_perv

`bb({eyes:"suspect", body:"two_up", mouth:"normal"})`

b: NÃO SEJAS TARADO. É CONTRA A LEI!

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: Lei dos Tarados, Secção 74.5: (1) Aquele que apreciar (a) aqueles ombros musculosos (b) aquele rabo redondo (2) será conhecido como

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: "UM TARADO NOJENTO"

```
_.a2_second_danger = 'law';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "the law";
```

(#act2c)

# act2b_louder_meaning

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: Na verdade, mesmo que encontres um propósito nobre na vida, *ainda* podes estragar tudo!

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Alfred Nobel queria paz mundial e que as culturas se entendessem. Então, decidiu tornar o ato de viajar mais fácil.

`bb({eyes:"normal_r"})`

b: Então, precisava de uma maneira barata de criar túneis para comboios. Então, inventou um material novo chamado "dinamite"...

`bb({body:"one_up", eyes:"normal"})`

b: que foi usado na Primeira Guerra Mundial para MATAR MILHÕES DE PESSOAS

`bb({body:"two_up", eyes:"shock"})`

b: É O EFEITO BORBOLETA, HUMANO! QUANTAS PESSOAS ESTÁS A MATAR ACIDENTALMENTE AGORA

```
_.a2_second_danger = 'butterfly';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "World War I";
```

(#act2c)

# act2b_different_social

`_.a2_first_choice = "different"`

`bb({eyes:"normal_r", body:"point", mouth:"normal"})`

b: Na verdade, sabes o que é pior do que ninguém gostar de ti? *Todos* gostarem de ti.

`bb({body:"one_up", eyes:"suspect", mouth:"normal"})`

b: Isto é, tornares-te alguém que só *procura* festa e prazer.

`bb({body:"normal", mouth:"small"})`

b: Uma vida superficial com amigos superficiais que só te conhecem superficialmente!

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Humano, precisamos de fugir destes zombies do prazer antes que eles nos transformem num deles!

```
_.a2_second_danger = 'zombies';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "zombies";
```

(#act2c)

# act2b_different_moral

`_.a2_first_choice = "different"`

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Há pessoas a morrer de fome e *genocídio* e nós estamos numa festa!

`bb({body:"point", eyes:"closed", mouth:"small"})`

b: Uma pessoa sábia uma vez disse: "a única coisa necessária para o triunfo do mal é que as boas pessoas não façam nada."

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: NÃO ESTAMOS A FAZER NADA.

`bb({mouth:"small"})`

b: AO ESTAR NESTA FESTA, ESTAMOS A AJUDAR O *HITLER*.

```
_.a2_second_danger = 'hitler';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "Hitler";
```

(#act2c)

# act2b_ignore

`_.a2_first_choice = "ignore"`

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Achas que estás seguro só porque tiraste as baterias do detetor de monóxido de carbono?

`bb({eyes:"suspect_r"})`

b: Nem vais sentir o cheiro do veneno! Vais só ficar com sono e depois mo--

`bb({body:"scream_c_1"})`

b: MORREEEERR

```
_.a2_second_danger = 'ignore';
_.a2_attack_2 = "harm";
_.a2_hoodie_callback = "carbon monoxide";
```

(#act2c)

# act2c

```
hong({body:"ignore_sweat"});
bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true});
```

b: ...

`bb({eyes:"happy", mouth:"smile", body:"chest"})`

b: Graças a Deus humano, acho que já me consegues ouvir!

`bb({eyes:"closed", body:"point"})`

b: TENHO DE TE AVISAR ACERCA...

{{if _.a2_first_choice=="louder"}}
[*Ainda mais* do mesmo perigo!](#act2c_louder)
{{/if}}

{{if _.a2_first_choice!="louder"}}
[*Mais* do mesmo perigo!](#act2c_louder)
{{/if}}

{{if _.a2_first_danger=="social"}}
[Um perigo social *diferente*!](#act2c_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[Um perigo moral *diferente*!](#act2c_different_moral)
{{/if}}

[Analisaste o ponche antes de beber?](#act2c_punch)

#act2c_louder

{{if _.a2_second_danger=="netflix"}}
(#act2c_louder_netflix)
{{/if}}

{{if _.a2_second_danger=="law"}}
(#act2c_louder_law)
{{/if}}

{{if _.a2_second_danger=="butterfly"}}
(#act2c_louder_butterfly)
{{/if}}

{{if _.a2_second_danger=="zombies"}}
(#act2c_louder_zombies)
{{/if}}

{{if _.a2_second_danger=="hitler"}}
(#act2c_louder_hitler)
{{/if}}

{{if _.a2_second_danger=="ignore"}}
(#act2c_louder_ignore)
{{/if}}

# act2c_louder_netflix

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: Na verdade, Netflix e take-out não é quarentena suficiente! Assim infetaríamos o sonhor das entregas!

`bb({body:"one_up", mouth:"small"})`

b: Precisamos de nos mudar para os territórios canadenses de Yukon e ter a nossa comida entregue por um drone!

`bb({body:"two_up", mouth:"normal"})`

b: Mas assim teriam que esterilizar o drone para livrá-lo dos nossos GERMES DE COITADINHOS

`_.a2_attack_3 = "alone";`

`_.a2_hoodie_callback = "a quarantine";`

(#act2d)

# act2c_louder_law

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: O TARADO será sentenciado a 72 horas num daqueles dispositivos medievais de humilhação pública

b: a menos que esteja secretamente *interessado* nesse tipo de coisa

`bb({body:"scream_a_1"})`

b: porque é um tarado nojento

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "the law";`

(#act2d)

# act2c_louder_butterfly

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: EFEITO BORBOLETA! Estás a usar um copo de plástico não biodegradável?

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: BAAM, UM ATERRO VAZ VENENO E MATA UMA CRIANÇA

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: Estás a suar e o teu coração está a bater com mais força?

`bb({body:"scream_a_1"})`

b: BAAM, LEVASTE O NOSSO SISTEMA DE SAÚDE À FALÊNCIA E MILHÕES MORRERAM

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "the butterfly effect";`

(#act2d)

# act2c_louder_zombies

`bb({body:"normal", mouth:"small", eyes:"angry"})`

b: Estes zombies do prazer vão tropeçar na tua direção a resmungar,

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: GOSTOOOOOS. GOSTOOOS.

`bb({body:"scream_a_1"})`

b: Depois vão MORDER-TE e transformar-te num MANO SEM CÉREBRO / ou numa VADIA FRAQUINHA!

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "zombies";`

(#act2d)

# act2c_louder_hitler

`bb({body:"scream_a_1"})`

b: OS NAZIS ESTÃO A VOLTAR ÀS RUAS NESTE MOMENTO

`bb({body:"one_up", mouth:"smile", eyes:"happy"})`

b: *Ainda bem que essa 'Boa Gente' se descuidou com coisas como 'relaxar' e 'cuidar de si'!*

`bb({body:"point", mouth:"smile", eyes:"happy_r"})`

b: *Agora os nossos planos podem ficar em quarto lugar!*

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "Hitler";`

(#act2d)

# act2c_louder_ignore

`bb({body:"normal", mouth:"normal", eyes:"normal_r"})`

b: Pensando bem, sabemos se este prédio *tem* um detetor de monóxido?!

`bb({body:"two_up", mouth:"small", eyes:"normal"})`

b: E se estivermos a ser envenenados *NESTE MOMENTO?*

`bb({body:"scream_a_1"})`

b: NEM ÍAMOS VER A MORTE A CHEGAR. ÍAMOS SIMPLESMENTE DEIXAR DE EXISTIR PARA SEMPR--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "carbon monoxide";`

(#act2d)

# act2c_different_social

`bb({body:"normal", mouth:"normal", eyes:"sad"})`

b: E se formos *fundamentalmente incapazes* de ser amados ou de amar outra pessoa?

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: E se algo partiu irreversivelmente dentro de nós há muito tempo? Ou nunca sequer existiu em nós em primeiro lugar?

`bb({body:"scream_a_1"})`

b: AHH ESTAMOS ESTRAGADOS! TÃO ESTRAGADOS TÃO ESTRAGADOS TÃO ESTR-

`_.a2_attack_3 = "alone";`

(#act2d)

# act2c_different_moral

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: E se estivermos *fundamentalmente podres?*

`bb({body:"one_up", eyes:"sad"})`

b: Outros têm um impulso interior para fazer o bem, mas nós só fazemos o "bem" por culpa ou vergonha, se tanto.

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: E se for da nossa natureza magoar os outros? E se não conseguirmos ser mais *que* um fardo para quem nos é próximo?

`bb({body:"scream_a_1"})`

b: AHH ESTAMOS ESTRAGADOS! TÃO ESTRAGADOS TÃO ESTRAGADOS TÃO ESTR-

`_.a2_attack_3 = "bad";`

(#act2d)

# act2c_punch

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Não estou a ser irracional. As pessoas *fazem* canecas de ponche com droga. É algo real que realmente acontece.

`bb({eyes:"suspect"})`

b: Humano, dói-te a cabeça? Custa-te mexer? Acho que estamos a morrer.

`bb({body:"scream_a_1"})`

b: AHHH ESTAMOS A MORRER! ESTAMOS A MORRER ESTAMOS A MO--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "punch bowls";`

(#act2d)

# act2d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"attacked"});
attack("20p", _.a2_attack_1);
```

(...401)

```
hong({body:"attacked_2"});
attack("20p", _.a2_attack_2);
```

(...401)

```
hong({body:"attacked_3"});
attack("20p", _.a2_attack_3);
```

(...1001)

h: M^EEERDA^!

h: MER^RRRR^DAA MER*^RRRRDAA^*

`bb({body:"two_up", mouth:"smile", eyes:"happy"});`

b: Yey, humano! Estou tão feliz por me conseguires ouvir!

`bb({body:"normal", mouth:"small", eyes:"sad"})`

b: Porque é que me estás a ignorar?

`hong({body:"facepalm"})`

h: Deus me livre, seu grande parvo.

`hong({body:"facepalm_2"})`

h: Conheces aquela história do nativo americano?

h: "Existem dois lobos dentro de ti, um é a esperança, o outro é o desespero, que lobo ganha? Aquele que alimentas."

```
hong({body:"facepalm_3"});
bb({eyes:"normal"});
```

h: Eu estava a tentar *matar-te à fome* , seu ^cabrão^ sádico!

`hong({body:"smile", mouth:"smile"})`

h: Que se ^foda^, em vez disso vou fazer afirmações positivas.

h: *Eu sou amado. Eu sou bom. Eu sou inteligente. Eu sou atraente. Eu sou especial.*

`bb({eyes:"suspect"});`

[Jesus, isso é tão narcisista!](#act2d_narcissist)

[Sabes que as afirmações positivas foram *refutadas?*](#act2d_disproven)

[Omg não credites histórias aleatórias para povos indígenas](#act2d_racist)

# act2d_disproven

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Na verdade, elas saem *pela culatra* às pessoas com baixa autoestima!

`bb({body:"one_up", mouth:"small", eyes:"normal"})`

b: Foi um estudo bem estruturado, um ensaio ao calhas controlado, o pesquisador não sabia quem era quem em que grupo.

`bb({body:"two_up", mouth:"small", eyes:"normal_r"})`

b: Resultados: se já tens baixa autoestima, pedir-te para repetir afirmações faz-te sentir *pior* do que se não tivesses dito nada!

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Wood 2009, Ciência Psicológica. Procura no Google Acadêmico, humano,

`bb({body:"scream_b_1"})`

b: ENTÃO PARA DE DIVULGAR NOTÍCIAS NÃO CIENTÍFICAS FALSAS 

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_narcissist

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: *Precisas* de, humildemente, ver as tuas próprias falhas para crescer como pessoa!

`bb({body:"two_up", eyes:"suspect"})`

b: Não podes simplesmente borrifar spray aromático numa sala que cheira a mofo! Cobrir as tuas falhas torna-te pior a longo prazo.

`bb({body:"chest", mouth:"smile", eyes:"closed"})`

b: Felizmente, eu, como o teu Lobo de Guarda, posso alertar-te sobre as tuas falhas. E agora, es-

`bb({body:"scream_b_1"})`

b: TUDO. ESTÁ TUDO MAL

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_racist

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Os nativos americanos são *pessoas reais* e não "selvagens nobres" que podes mencionar para tornar os teus conselhos mais *exóticos*.

`bb({eyes:"suspect_r"})`

b: Estás a reduzir pessoas individuais e culturas complexas a um cartão do Hallmark! Isso é "racismo benevolente"!

`bb({body:"scream_b_1"})`

b: PARA DE SER RACISTA Ó IDIOTA ESTRÁBICO

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2e

h: ^CABRÃO^.

`hong({body:"yell", mouth:"yell"})`

h: Sabes que mais? Tu és *irracional*.

h: Toda a gente sabe que as emoções são irracionais! Principalmente o medo!

`hong({body:"facepalm_2"})`

h: Não passas de restos evolutivos inúteis, como o apêndice ou os dentes do siso!

`hong({body:"yell", mouth:"yell"})`

h: ^Caralho^, essa metáfora do lobo é estúpida! És apenas um monte de neuro-químicos na minha cabeça.

`hong({body:"cross", mouth:"cross"})`

h: Então, porque é que haveria de ouvir um pedaço de ^merda^ inútil, irracional e inexistente como tu?!

`bb({eyes:"sad", MOUTH_LOCK:true})`

b: ...

[Jesus, humano. Isso é muito ofensivo.](#act2e_hurtful)

[Eu sou um sentimento. Os sentimentos são válidos.](#act2e_valid)

[Humano, nós *os dois* somos "apenas químicos".](#act2e_rational)

# act2e_hurtful

`bb({body:"chest"})`

b: Eu sou *parte* de ti, sabes? Quando dizes isso, estás a magoar-te a *ti próprio*.

`bb({body:"scream_a_1"})`

b: Porque é que te estás a magoar, humano? PARA DE TE MAGOAR.

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2e_rational

`bb({body:"normal", mouth:"normal", eyes:"normal_r"});`

b: As tuas motivações mais profundas são dopamina, e as tuas maiores alegrias são serotonina.

`bb({body:"one_up"});`

b: As tuas memórias são pesos sinápticos, a tua razão são sinais elétricos propensos a falhas.

`bb({eyes:"normal", body:"normal"});`

b: Então, se ser "apenas um químico" significa que *sou* irracional... isso significa que *tu és* irracional!

`bb({body:"two_up", eyes:"shock"});`

b: E se *ambos* formos irracionais, *nunca* descobriremos como é ser-se realizado e feliz!

`bb({body:"scream_a_1"})`

b: AHHH ESTAMOS ESTRAGADOS! TÃO ESTRAGADOS TÃO ESTRAGADOS TÃO ESTR--

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2f)

# act2e_valid

`bb({body:"normal", mouth:"normal", eyes:"suspect"});`

b: Espera aí... "eles" dizem que os sentimentos são válidos, que tu deves sempre aceitar as tuas emoções.

`bb({eyes:"suspect_r"});`

b: Mas "eles" também dizem que as emoções são irracionais, que as emoções não são confiáveis.

`bb({eyes:"angry"});`

b: Oh meu Deus, "eles" estiveram a mentir-nos este tempo todo!

`bb({body:"scream_a_1"})`

b: "ELES" ALIMENTAM-NOS COM CONTRADIÇÕES PARA NOS FAZER DEPENDENTES DO COMPLEXO INDUSTRIAL DE AUTO-AJUDA

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2f

`hong({body:"defeated", MOUTH_LOCK:true});`

h: ...

h: Eu odeio isto. Deus, dói tanto. *Odeio* isto.

h: Eu não te posso apaziguar. Eu não te posso ignorar. Eu não posso lutar contigo.

`bb({eyes:"suspect"});`

h: Não importa o que eu faça, não consigo me livrar de t--

`bb({body:"cry_1"});`

b: Bem, talvez *NÃO* DEVAS LIVRAR-TE DE MIM.

`bb({body:"cry_2"});`

b: Como achas que *eu* me sinto, humano?!

`bb({body:"cry_4", mouth:"cry", eyes:"cry"})`

b: Estou a dar o meu melhor para ser o teu Cão de Guarda, mas tu continuas  a ver-me como um Lobo Mau!

b: Então eu tento alertar-te ainda *mais* sobre o perigo! *Mais* perigo! Perigo* diferente*!

`bb({eyes:"cry_2"})`

b: Mas não importa o quanto eu tente proteger-te, *ainda* pensas que sou teu inimigo!

`bb({body:"cry_5"});`

b: O que estou a fazer de errado?

`bb({body:"cry_2"});`

b: Eu *sei que* sou péssimo no meu trabalho. Mas estou *a tentar*, humano!

`bb({body:"cry_3"});`

b: ...Estou a tentar.

`bb({body:"cry_6", mouth:"right", eyes:"cry_r_1"});`

b: Não tens de prestar atenção aos meus avisos, nem concordar comigo, nem mesmo *gostar* de mim.

`bb({eyes:"cry_r_2"});`

b: Eu... tudo o que quero é que sejas paciente comigo.

`bb({eyes:"cry_r_3"});`

b: Só quero que te mantenhas ao meu lado, em vez de desapare-

```
bb({eyes:"cry_r_4"});
hong({body:"listen"});
```

r: Hey.

```
hong({body:"look"});
Game.clearText();
publish("act2-in-2");
publish("hp_hide");
music('party1', {volume:0.4, fade:2});
```

(...2000)

```
publish("act2",["party_hunter",2]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Parece que estás a discutir contigo mesmo, miúdo.

```
publish("act2",["party_hunter",3]);
publish("act2",["party_hong",13]);
```

h2: Era assim tão óbvio?

```
publish("act2",["party_hunter",4]);
publish("act2",["party_hong",14]);
```

r: Estavas, uh, a resmungar com a tua sweat sobre {{_.a2_hoodie_callback}} ou algo assim.

```
publish("act2",["party_hunter",13]);
publish("act2",["party_hong",15]);
sfx("rustle", {volume:0.6});
setTimeout(function(){
	publish("act2",["party_hong",16]);
	sfx("concrete_step3", {volume:0.6});
},401);
setTimeout(function(){
	publish("act2",["party_hong",17]);
	sfx("concrete_step4", {volume:0.6});
},801);
```

h2: Oh Deus, estou uma desgraça.

```
publish("act2",["party_hunter",7]);
publish("act2",["party_hong",18]);
sfx("squeak");
```

r: Ei. Não estás sozinho, amigo. A ansiedade é muito comum.

```
publish("act2",["party_hunter",5]);
publish("act2",["party_hong",19]);
```

{{if _.act1_ending=="fight"}}
r: Raios, ainda ontem, ouvi que alguém no campus teve um colapso nervoso e partiu o telemóvel!
{{/if}}

{{if _.act1_ending=="flight"}}
r: Raios, ainda ontem, ouvi que alguém se enrolou como um tatu e chorou em público!
{{/if}}

```
publish("act2",["party_hunter",2]);
```

r: Ouve: eu sei o que é ter aquele animal na cabeça.

```
publish("act2",["party_hunter",8]);
```

r: *Todos* nós sabemos. É por isso que dou estas festas todos os fins de semana, para esquecer as preocupações, esquecer aquele bicho.

```
publish("act2",["party_hunter",9]);
publish("act2",["party_hong",20]);
```

h2: Mas a minha ansiedade...

```
publish("act2",["party_hunter",2]);
publish("act2",["party_hong",21]);
```

r: Não te preocupes, miúdo. Eu costumava ser como tu. Mas depois descobri um pequeno truque para fazer aquela voz negativa calar a boca para sempre...

```
publish("act2",["party_hunter",3]);
Game.clearText();
music(null, {fade:1});
```

(...2001)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",22]);
sfx("rustle");
```

(...2501)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",23]);
sfx("rustle2");
```

(...1001)

```
publish("act2",["party_hunter",11]);
```

r: A minha própria mistura especial. É um pouco mais forte do que... bem, do que qualquer coisa legal, na verdade.

```
publish("act2",["party_hunter",12]);
publish("act2",["party_hong",24]);
```

r: Bota abaixo, ^cabras^!

```
hong({body:"hold"});
bb({body:"normal", mouth:"small", eyes:"wat"});
Game.clearText();
Game.WORDS_HEIGHT_BOTTOM = -1;
publish("act2-out-3");
publish("hp_show");
```

(...3500)

[Oh meu Deus.](#act2g_1) `Game.OVERRIDE_CHOICE_LINE=true`

[Este é um mecanismo de coping terrível.](#act2g_2) `Game.OVERRIDE_CHOICE_LINE=true`

[Não aceites bebidas de estranhos.](#act2g_3) `Game.OVERRIDE_CHOICE_LINE=true`

# act2g_1

b: O--

(#act2g)

# act2g_2

b: T--

(#act2g)

# act2g_3

b: D--

(#act2g)

# act2g

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"forward", mouth:"forward"});
bb({body:"frazzled", mouth:"frazzled", eyes:"frazzled"});
```

h: Mmm, que sabor requintado!

h: Um sabor encorpado de "acalma a tua mente", com um gosto subtil de "nunca mais sintas nada"!

b: Isto é mau, humano. Isto é muito, muito mau.

[É assim *que* o vício começa.](#act2h_opt1) `Game.OVERRIDE_CHOICE_LINE=true`

[Eu *sabia que* o anfitrião era profundamente doido!](#act2h_opt3) `Game.OVERRIDE_CHOICE_LINE=true`

[Além disso, ele pode ter posto drogas nisso!](#act2h_opt2) `Game.OVERRIDE_CHOICE_LINE=true`


# act2h_opt1

b: É *assi-*

(#act2h)

# act2h_opt2

b: Além disso, ele po--

(#act2h)

# act2h_opt3

b: Eu *sabia* qu--

(#act2h)

# act2h

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"back", mouth:"back"});
bb({body:"panicked", mouth:"panicked", eyes:"panicked"});
```

h: Delicioso, *e* mais barato que terapia!

b: HUMANO, POR FAVOR, PARA

h: Hehehe!

h: E o que é que *tu* vais fazer acerca disso, ^cabrão^?

b: Desculpa, humano.

b: Vou ter que usar o meu ATAQUE ESPECIAL

```
bb({body:"special_a"});
music('battle', {volume:0.5});
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act2h_attack) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act2h_attack) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act2h_attack) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`

# act2h_attack

```
bb({body:"special_b_1"});
hong({body:"forward", mouth:"forward"});
sfx("charging");
```

h: O que é esta ^merda^?

h: Vais berrar-me mais *palavras* estúpid--

```
bb({body:"special_c"});
sfx("hadouken");
```

(...901)

(#act2i)

# act2i

```
publish("hide_tabs");
publish("show_special_attack");
Game.FORCE_CANT_SKIP = true;
music(null);
stopAllSounds();
```

(...5000)

```
publish("show_tabs");
hong({ body:"final", mouth:"final" });
bb({ body:"normal", mouth:"normal", eyes:"sad" });
attack("100p", _.SPECIAL_ATTACK);
Game.FORCE_CANT_SKIP = false;
setTimeout(function(){
	publish("remove_special_attack");
},30);
```

(...2500)

h: QUE ^CARALHO^ FOI ISTO

b: Desculpa. Eu precisava de te mostrar as consequências.

{{if _.SPECIAL_ATTACK == "harm"}}
h: EU PODIA *VER O* MEU PRÓPRIO CADÁVER. CONSEGUIA *TER* A SENSAÇÃO DE ESTAR MORTO. 
{{/if}}

{{if _.SPECIAL_ATTACK == "alone"}}
h: CONSEGUIA *SENTIR* O OLHAR DE NOJO DE TODOS. CONSEGUIA *OUVIR* TUDO O QUE DIZIAM.
{{/if}}

{{if _.SPECIAL_ATTACK == "bad"}}
h: CONSEGUIA *OUVIR* AS MINHAS COSTELAS A PARTIR. CONSEGUIA *SENTIR O SABOR* DO SANGUE.
{{/if}}

b: Desculpa, humano.

n: ACABA COM ELE

[{LUTA: Dá um soco ao anfitrião.}](#act2j_fight) `Game.OVERRIDE_CHOICE_LINE=true`

[{FOGE: Vamos sair daqui.}](#act2j_flight) `Game.OVERRIDE_CHOICE_LINE=true`

# act2j_fight

`bb({ eyes:"angry" });`

b: Aquele psicopata estava a aproveitar-se de ti.

b: Ele estava a tentar corromper-te, tornar-te tão louco quanto ele!

`bb({ body:"yell_angry_1" });`

b: Dá um soco àquele idiota! Acaba com ele!

`bb({ body:"final_1" });`

b: DÁ-LHE UM SOCO DÁ-LHE UM SOCO DÁ-LHE UM SOCO DÁ-LHE UM SOCO DÁ-LHE UM S--

`_.a2_ending = "fight";`

(#act2k)

# act2j_flight

b: Eu *sabia que* este festivaleiro era profundamente louco. Ele adormece a dor com coisas horríveis!

`bb({ body:"yell_1" });`

b: E está a enganar-te para fazeres a mesma coisa! Ele está a corromper-te! Temos que te libertar.

`bb({ body:"final_1" });`

b: VAI EMBORA VAI EMBORA VAI EMBORA VAI EMBORA VAI EMBORA VAI EMBO--

`_.a2_ending = "flight";`

(#act2k)

# act2k

```
Game.clearText();
publish("act2-in-4");
publish("hp_hide");
music('party1', {volume:0.6, fade:1.5});
```

(...2001)

```
publish("act2",["party_hong",26]);
sfx("slide");
```

(...1001)

```
publish("act2",["party_hunter",14]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Estás bem, miúdo?

`publish("act2",["party_hunter",13]);`

{{if _.a2_ending=="fight"}}
(#act2k_fight)
{{/if}}

{{if _.a2_ending=="flight"}}
(#act2k_flight)
{{/if}}

# act2k_fight

```
Game.clearText();
publish("act2",["party_hunter",21]);
publish("act2",["party_hong",33]);
music(null);
sfx("hit");
```

(...1000)

```
sfx("record_scratch");
publish("act2",["party_hunter",22]);
publish("act2",["party_hong",34]);
publish("act2",["dee",6]);
publish("act2",["dum",6]);
```

r: T-tu...

```
publish("act2",["party_hunter",23]);
publish("act2",["party_hong",35]);
publish("act2",["dee",5]);
publish("act2",["dum",5]);
music('party1', {volume:0.6, fade:6});
```

r: És *tarado*.

r: Gosto disso. Anda à minha festa no próximo fim-de-semana, fofo.

```
publish("act2",["party_hunter",19]);
publish("act2",["party_hong",36]);
```

h2: Ok adeus, ciao, adios, au revoir

r: O animal pode ter vencido hoje, mas volta, e vou preparar algo ainda mais forte para ti!

h2: Sayōnara, auf wiedersehen, zài jiàn, shalom

r: Tu e eu, miúdo, vamos mostrar àquela besta quem manda!

(#act2k_end)

# act2k_flight

`publish("act2",["party_hong",36]);`

h2: ok desculpa, tenho de ir

`publish("act2",["party_hunter",16]);`

r: Que ^merda^. O animal ganhou hoje, uh?

`publish("act2",["party_hunter",15]);`

h2: Não, não, eu só, uh, tenho de ir correr uma maratona. Tenho de ir embora.

`publish("act2",["party_hunter",19]);`

r: Anda à minha festa no próximo fim-de-semana, fofo. Vou preparar algo ainda mais forte para ti.

h2: Ok, obrigado, tenho que correr, correr, correr, correr, correr

r: Tu e eu, miúdo, vamos mostrar àquela besta quem manda!

(#act2k_end)

# act2k_end

```
Game.clearText();
publish("act2-out-5");
publish("act2-outro", ["end1"]);
music("hum", {fade:2, volume:0.6});
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2500)

```
publish("act2", ["act2_end",2]);
sfx("whoosh");
```

(...1000)

b: Humano! Estás bem?

```
publish("act2", ["act2_end","next"]);
```

b: Deus, aquilo foi *intenso.* Nós realmente podíam--

```
Game.clearText();
publish("act2", ["act2_end","next"]);
music(null);
sfx("squeak");
```

(...1500)

```
publish("act2", ["act2_end","next"]);
sfx("hit");
```

(...1000)

h: Vou voltar à festa no próximo fim-de-semana.

h: Da próxima vez que lutarmos, não vou apenas *derrotar-te*...

h: Eu vou *matar-te* ^caralho^.

```
Game.clearText();
publish("act2", ["act2_end","next"]);
sfx("concrete_step1");
````

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step2", {volume:0.8});
```

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step3", {volume:0.5});
```

(...901)

`sfx("concrete_step4", {volume:0.25});`

(...3000)

`_.INTERMISSION_STAGE = 2;`

(#intermission)