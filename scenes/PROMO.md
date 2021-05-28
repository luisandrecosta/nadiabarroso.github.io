# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[JOGAR!](#intro-start)`publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Então, antes de começarmos, como *gostarias* de ler?

`publish("show_options_bottom")`

# intro-start-2

n3: Agora, vamos começar a história...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: ISTO É UM HUMANO

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: E ESTA É A ANSIEDADE DO HUMANO

n: _TU_ ÉS A ANSIEDADE

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Não. Não, não, não estou a ouvir. Vou olhar o meu telemóvel.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: O TEU TRABALHO É PROTEGER O TEU HUMANO DO *PERIGO*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Eia! Estás a desperdiçar o teu tempo no Twitter! Outra vez!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Sim, eu pergunto-me por que não me sento e ouço os meus pensamentos com mais frequência.

`hong({eyes:"neutral"});`

n: RÁPIDO, AVISA-O SOBRE UM *PERIGO!*

```
bb({eyes:"look"});
```

[Oh não, olha para esta notícia horrível!](#act1d_news)

[Oh não, este tweet é secretamente sobre *nós?*](#act1d_subtweet)

[Ei, um GIF de um gato a beber leite](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Heh ya que fofo, eu--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: OS GATOS NÃO CONSEGUEM DIGERIR O LEITE E SOMOS HORRÍVEIS POR APRECIAR ABUSO ANIMAL

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



