# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: Saúde!

```
publish("act3",["roofhunter",1]);
publish("act3",["roofhong",1]);
sfx("drinking");
```

(...4001)

```
publish("act3-alpha", ["dizzyhunter",1]);
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",3]);
```

h2: *Ah*, isto sabe tão bem.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: Sabes miúdo...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: Especificamente, onde sabe melhor é nas minhas amígdalas.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: Relembras-me a mim quando era mais novo. Na época em que era atormentado pelo animal na minha cabeça.

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: Estou tão grato que posso passar conhecimento e ajudar-te a matar a tua besta como matei a minha.

```
publish("act3",["roofhunter",2]);
```

r: Ei, pergunta rápida: verdade ou conse--

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: CONSEQUÊNCIA!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: Haha! Boa.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: Ok. Está a ver aquela piscina lá embaixo?

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: Sim? Seis andares abaixo?

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: Salta.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: Espera, o quê?

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: O animal começou a choramingar, não foi?

```
publish("act3",["roofhunter",23]);
```

r: *Oh nãooooo é perigoso, não faças issooo.*

```
publish("act3",["roofhunter",22]);
```

r: Mas é exatamente por isso que precisamos de emoções que desafiem a morte! Diverte-te! Carpe diem! Vamos snifar coca no ^cu^ de uma prostituta, #YOLO!

```
publish("act3",["roofhunter",10]);
```

r: Mostrar àquele animal que nós não queremos saber da *^merda^* que ele diz! Salta.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: Uh, mas às vezes, hum... o medo tem razão...

```
publish("act3",["roofhunter",5]);
publish("act3",["roofhong",12]);
music(null, {fade:2});
```

r: ...

```
publish("act3-alpha", ["dizzyhunter",0]);
publish("act3",["roofhunter",6]);
publish("act3",["dd",1]);
```

r: Desculpa, caíste nessa propaganda da "McMindfulness" que afirma que sentirmo-nos mal é *bom?*

```
publish("act3",["roofhunter",17]);
```

r: Os ^cabrões^ que dominam este mundo dão ao resto de *nós* ansiedade e depressão,

```
publish("act3",["roofhunter",18]);
```

r: E depois fazem TED Talks para nos dizer para "aceitar" ser ^fodido^ e "abraçar" aquele demônio sádico nas nossas cabeças!

```
publish("act3",["roofhunter",6]);
```

r: Miúdo, eu sei que *tu* sabes que esse animal *magoa* gente como nós. *Tortura* pessoas como nós.

```
publish("act3",["roofhunter",19]);
```

r: Não é nosso amigo. É uma besta raivosa, que precisa de ser *tranquilizada*,

```
publish("act3",["roofhunter",20]);
```

r: Ou de levar com uma *bala no crânio*.

```
publish("act3",["roofhunter",27]);
```

r: Caso contrário, vais deixá-lo vencer.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: Não. Estás enganado.

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
	music('battle_dark_loop');
});
```

h2: Não o vou deixar vencer.

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: Sim, ^caralho^! Acredito em ti, baby! Mata-o! <3

(#act3a)



# act3a

```
Game.clearText();
publish("act3-out");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
_.act3_bb_body = 1;
```

(...1500)

```
publish("hp_show");
```

b: não não não não não não

n: ESTE CAPÍTULO TEM DOIS FINAIS POSSÍVEIS. UM É *MUITO, MUITO MAU.*

b: NÃO NÃO NÃO NÃO NÃO NÃO NÃO NÃO NÃO NÃO NÃO NÃO NÃO NÃO

n: ESCOLHE COM SABEDORIA. PROTEGE O TEU HUMANO

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: AAAAAAAAAAAAAAAAAA

`bb({ mouth:"normal" });`

n: BOA SORTE

```
Game.clearText();
bb({ eyes:"start" });
```

[Humano, podes mesmo MORRER aqui!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[Isto é estúpido e autodestrutivo!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[Estes malucos não são realmente teus amigos!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: H--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: T--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: T--

(#act3a_after)

# act3a_after

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Sabes, eu podia ter acreditado em ti... se já não tivesses tentado isso um milhão de vezes.

h: Tu és o lobo que gritou lobo.

```
bb({ eyes:"sad" });
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act3_fork) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act3_fork) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act3_fork) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`


# act3_fork

```
Game.clearText();
bb({body:"special_attack"});
sfx("charging");
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
Game.FORCE_CANT_SKIP = false;
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Também tentaste isso.

b: Humano, por favor...

`hong({ eyes:"look_right" });`

h: *Desculpa lá* se a Big Pharma não aprova a minha automedicação.

h: Olha, ^cabrão^, *todos* nós temos uma maneira de te calar a boca, ^caralho^.

`hong({ body:"look_up", eyes:"look_up" });`

h: Algumas pessoas atiram-se ao trabalho.

`hong({ body:"look_down", eyes:"look_down" });`

h: Algumas pessoas dedicam-se ao sexo, às drogas e à atualização do feed do Facebook.

`hong({ body:"normal", eyes:"look_right" });`

h: Algumas pessoas atiram-se a outras pessoas.

`hong({ eyes:"angry" });`

h: Vou atirar-me para a piscina.

[Estás bêbado e a piscina está SEIS ANDARES ABAIXO](#act3_bad_1_harm)

[Bolas, este é o agradecimento que recebo?!](#act3_bad_1_insult) `bb({eyes:"angry"});`

[Está bem, eu admito. Eu estraguei tudo.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: Mesmo se caíres na água, a tensão superficial vai partir as tuas costelas e causar *no mínimo* uma concussão!

h: Eh.

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Eu vi um russo fazer isto no YouTube uma vez.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: Com licença, o *obrigado?*

`bb({ eyes:"angry" });`

b: É exatamente por causa d isto que eu *existo!* Porque os humanos não são confiáveis para se protegerem!

b: Tenho tentado proteger-te durante toda a minha vida e agora va--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)

# act3_good_1

`hong({ body:"laugh_1" })``

h: heh.

`hong({ body:"laugh_2" })``

h: hahahaha

`hong({ body:"laugh_3" })``

h: HAHAHAHAHAHA

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: Oh, uau, esse é o maior *^filho da puta^* de eufemismo do século!

`hong({ body:"yell_2" });`

h: Sim, seu monte de ^merda^ coberto de sangue! ^Fodeste^ tudo!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: Mais alguma observação, Capitão Óbvio?

[Mas vingança contra mim não é a resposta!](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Mas desta vez estou *certo*!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Eu magoei-te.](#act3_good_2a)


# act3_good_1_fail_revenge

b: Precisas de ter um relacionamento mais saudável com as tuas emoções, em vez de as afogar com--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)



# act3_good_1_fail_harm

b: Então, por favor, baixa a garrafa e vam--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)




# act3_bad_2

`bb({ eyes:"sad" });`

b: por favor... não...

h: A tua barra de energia está terrivelmente baixa, lobo.

h: Se fosse a ti, escolhia as tuas próximas palavras com muito cuidado.

`bb({ eyes:"normal" });`

[Muito bem. Cansei-me de te proteger.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[Estive sempre certo.](#act3_bad_2_right)

[Desculpa.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: Então, vai e salta. Vê se me importo.

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: Está bem, então. Bota abaixo.

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: NÃO, ESPERA! ERA PSICOLOGIA REVERSA, ERA SUPOSTO FAZERES O *OPOSTO* DO QUE EU DIS--

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: *Estás* a colocar-te em perigo. Os teus supostos amigos *estão* a usar-te. E *tu* estás a usar os teus queridos amigos.

`bb({ eyes:"sad" });`

b: Então, por favor, humano... porquê não acreditas em mim?!

h: Porque nunca acreditaste em *mim*.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: Outros Lobos de Guarda têm humanos que dedicam tempo para treiná-los pacientemente, para *aprenderem* a trabalhar juntos,

b: Em vez de os odiarem por tentarem protegê-los! Então, porquê é que não podes simplesm--

`bb({ eyes:"normal" });`

h: Resposta errada.

(#act3_bad_3)



# act3_bad_3

```
music(null);
hong({body:"drink"});
bb({body:"attacked"});
publish("bb_STOP_VIBRATING");
attackBB("100p");
```

(...2000)

```
hong({ body:"normal", mouth:"normal", eyes:"normal" });
bb({ body:"dead" });
```

(...999)

h: *"A única coisa a temer é o medo em si."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"Não te preocupes, sê feliz!"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: Todos os sábios do nosso tempo concordam: emoções negativas são *más!*

`hong({ eyes:"less_angry" });`

h: Duh! É por isso que se chamam *negativas!*

b: Humano, por favor...

`hong({ eyes:"normal" });`

h: Uma altura disse: “Eu só me quero livrar de toda esta dor.”

h: O meu desejo realizou-se. Já não sinto dor, medo, nem ansiedade...

h: Não sinto absolutamente nada.

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: Eu estava tão obcecado em garantir que nada mais te magoava, que não percebi que era *eu* que te estava a causar dor.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: NÃO. ME^RDA^.

`hong({ body:"yell_1" });`

h: ^FODA-SE^. Demoraste mesmo assim tanto para finalmente perceber isso?!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: Podias ter-nos poupado tantos problemas, seu grande adorável ^cabrão^. Porquê é que não percebeste isso antes?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...tu *sentes muito.*

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: Sentes muito pelo *quê*?

(#act3_good_2q)


# act3_good_2q

`bb({mouth:"sorry", eyes:"sorry"});`

{{if _.apologized_for_hurt}}
(#act3_good_2q_already_apologized)
{{/if}}

{{if !_.apologized_for_hurt}}
(#act3_good_2q_not_already_apologized) 
{{/if}}


# act3_good_2q_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"less_angry" });`

[Desculpa não ter sido um bom protetor.](#act3_good_3_protector)

[Desculpa por não te ter respeitado.](#act3_good_3_respect)

[Desculpa.](#act3_good_4)


# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[Desculpa por ter um humano terrível!](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[Desculpa por não te ter respeitado.](#act3_good_3_respect)

[Desculpa por te ter magoado.](#act3_good_3_hurt)



# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: É o meu dever alertar-te acerca do perigo *real*, mas continuei a ladrar para os carros e para o carteiro.

`bb({eyes:"sorry_up"});`

b: A ladrar para as sombras. A ladrar tanto.

`bb({eyes:"sorry"});`

b: Faz sentido que me queiras amordaçar.

`bb({eyes:"sorry_down"});`

b: Desculpa.

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: Eu devia ser *o teu* fiel Cão de Guarda, mas agi como se tu é que *me* devesses obedecer.

`bb({eyes:"sorry_up"});`

b: Há uma diferença entre protetor e diretor de prisão, e eu ultrapassei o limite.

`bb({eyes:"sorry_down"});`

b: Desculpa.

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: Eu estava tão obcecado em tentar proteger-te, que nunca parei para pensar que *eu* te estava a magoar.

`bb({eyes:"sorry_up"});`

b: Eu fui um cão mau.

`bb({eyes:"sorry_down"});`

b: Desculpa.

(#act3_good_4)


# act3_good_4

```
music(null,{fade:3});
hong({ eyes:"less_angry", MOUTH_LOCK:true },0);
```

h: ...

```
hong({ body:"stop", mouth:"stop", eyes:"blank" });
```

h: Sim, bem, isto foi uma ideia estúpida de qualquer maneira.

h: Eu só fiz isto para mexer contigo e, bem, consegui.

h: Vamos dizer que é um empate, ok?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: Ok.

h: Ok.

n: *EMPATE*

`_.a3_ending = "walkaway";`

(#act3_end)









# act3_end

```
Game.clearText();
publish("act3-in");
publish("hp_hide");
Game.FORCE_CANT_SKIP = true;
```

{{if _.a3_ending=="walkaway"}}
(#act3_walkaway)
{{/if}}

{{if _.a3_ending=="jump"}}
(#act3_jump)
{{/if}}






# act3_walkaway

```
publish("start-walkaway-anim");
Game.WORDS_HEIGHT_BOTTOM = 205;
```

(...3501)

```
sfx("bottle_toss");
publish('hong-next');
publish("act3",["roofhunter",7]);
```

(...667)

```
publish("act3",["dd",4]);
publish("act3",["roofhunter",26]);
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("concrete_step2");
```

(...667)

```
publish('hong-next');
publish("act3",["roofhunter",27]);
```

`Game.FORCE_CANT_SKIP = false;`

r: Oh *anda lá*. Depois de tudo o que aquele animal te fez, vais simplesmente *desistir?*

r: Qual é o problema, miúdo? Estás *assustado?*

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: Sim.

h2: Tenho medo.

`publish('hong-next')`

h2: Mas não faz mal!

`publish('hong-next')`

h2: Não há problema em ter medo.

`publish('hong-next')`

(...500)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1167)

```
publish('hong-next');
```

(...833)

```
publish('hong-next');
sfx("rustle2");
```

(...1333)

```
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",31]);
sfx("concrete_step4");
```

(...667)

```
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("door");
```

(...1333)

```
publish('hong-next');
sfx("concrete_step2");
```

(...501)

```
publish('hong-next');
Game.FORCE_CANT_SKIP = false;
sfx("lock_door");
publish("act3",["roofhunter",32]);
```

(...2001)

```
publish("act3",["roofhunter",33]);
```

r: Ele trancou a porta?

```
Game.clearAll();
_.INJURED = false;
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2000)

(#act4)




# act3_jump

```
publish("start-jump-anim");
Game.FORCE_TEXT_Y = 300;
```

(...2001)

```
publish('hong-next');
sfx("bottle_toss");
```

(...833)

```
sfx("concrete_step1");
sfx("claps");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",28]);
```
(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step2");
publish('hong-next');
publish("act3",["roofhunter",28]);
```

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",34]);
```

(...1167)

```
sfx("rustle2");
publish('hong-next');
```

(...1001)

`publish('hong-next')`

b: não...

(...501)

`Game.clearText();`

`publish('hong-next')`

(...1333)

```
sfx("quack");
publish('hong-next');
```

(...1333)

`publish('hong-next')`

b: não não não

(...501)

`Game.clearText();`

`publish('hong-next')`

(...2001)

```
sfx("rustle2");
publish('hong-next')
```

(...501)

```
sfx("concrete_step1");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",30]);
```

(...167)

```
sfx("concrete_step2");
publish('hong-next');
```

(...167)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",2]);
publish("act3",["roofhunter",15]);
```

(...167)

```
sfx("bottle_slip");
publish('hong-next');
publish("act3",["dd",3]);
publish("act3",["roofhunter",16]);
```

(...833)

```
sfx("rustle");
publish('hong-next');
```

(...167)

`publish('hong-next')`

(...167)

```
publish('hong-next');
Game.FORCE_TEXT_Y = 325;
Game.OVERRIDE_FONT_SIZE = 50;
```

b: NÃO!

(...400)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-injury-show");
publish("hide_tabs");
```

(...2000)

```
sfx("hospital1");
publish("act4-injury", [1]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital2");
publish("act4-injury", [2]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital3");
publish("act4-injury", [3]);
```

(...8000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...5500)

`_.INJURED = true;`

(#act4)
