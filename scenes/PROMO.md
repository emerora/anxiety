# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[JÁTÉK!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Mielőtt elkezdjük, hogyan szeretnél *olvasni*?

`publish("show_options_bottom")`

# intro-start-2

n3: Kezdődjék a történetünk...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: EZ EGY EMBER

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

n: ÉS EZ ITT AZ EMBER SZORONGÁSA

n: _TE_ VAGY A SZORONGÁS

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Nem. Nem, nem, nem hallak. Inkább megnézem a telefonom.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: A FELADATOD MEGVÉDENI AZ EMBERED A *VESZÉLYTŐL*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Ne! Elgörgeted az életed Twitteren! Megint!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Ja, nem is értem miért nem ülök és hallgatom a gondolataimat gyakrabban.

`hong({eyes:"neutral"});`

n: GYORSAN, FIGYELMEZTESD A *VESZÉLYRŐL!*

```
bb({eyes:"look"});
```

[Jaj ne, nézd azt a borzalmas hírt!](#act1d_news)

[Jaj ne, ez a poszt titkon *rólunk* szól?](#act1d_subtweet)

[Hé, egy GIF amin egy macska tejet iszik](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Hehe ja ez aranyos, É--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: A MACSKÁKNAK ÁRTA TEJ, MI MEG ÉLVEZZÜK A SZENVEDÉSÜKET. SZÖRNYŰEK VAGYUNK!

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



