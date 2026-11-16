# Violet Slopes

A Three.js snowboarding game themed on the Violet Flame of the Ascended Masters. Ride a 26 km mountain in five stages. Chain tricks, hoops and grinds to change the colour of your violet-fire trail, and finish on a giant ramp that launches you into the sun.

## Play

Everything lives in a single page. Open `index.html` through any static web server, for example:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

Three.js r160 loads from the jsDelivr CDN, so you need an internet connection. Use a local server rather than opening the file straight from disk. Browsers treat `file://` pages as cross-origin, and the music can come out silent. If the recording can't load at all, the game falls back to a built-in synthesized waltz.

## Controls

| Action | Keyboard | Controller |
| --- | --- | --- |
| Carve / spin in air | A D or ← → | Left stick / D-pad |
| Tuck / frontflip in air | W or ↑ | Stick up / RT |
| Brake / backflip in air | S or ↓ | Stick down / LT |
| Ollie, pop off rails | Space | A |
| Grabs (Indy, Melon, Method) | J K L / Shift | X, B, LB, RB |
| Violet Flame boost (meter full) | F | Y |
| Pause | P / Esc | Start |
| Music on/off · mute all | N · M | Back/Select |

## How it plays

- **Combos.** Tricks, hoops and grinds raise the multiplier. The fire trail changes through five tiers: Violet Spark, Violet Flame, Amethyst Blaze, Transmutation and Ascension. Points bank after 3 seconds without a new combo move.
- **Violet Flame boost.** Combo moves fill the meter. When it is full, the meter glows and a button prompt flashes. The boost gives 7 seconds of extra speed and double points, and you burn through trees instead of crashing into them.
- **The course.** It is the same fixed, seeded course every run. It curves more, gets steeper and fills with more obstacles as you descend. Along the way are steep walls ("Amethyst Wall"), cliff drops ("Leap of Faith") and rollers. Top speed is about 300 km/h in a tuck.
- **Lives.** You have five. Every wipeout costs one, and at zero you start over.
- **The ending.** The run funnels into a giant ramp that launches you into the violet sun, and **YOU WIN**.

## Credits

- Game code: generated with Claude.
- Engine: [three.js](https://threejs.org) (MIT), loaded from jsDelivr.
- Music: *The Blue Danube*, Op. 314 (Johann Strauss II), performed by Das Orchester Tsumugi / Takashi Inoue, live at Fukuoka Symphony Hall, 10 March 2024. Recording courtesy of [www.classicals.de](https://www.classicals.de), licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). The file in `music/blue-danube.mp3` is unmodified (renamed only).
