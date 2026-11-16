# Violet Slopes

A Three.js snowboarding game themed on the Violet Flame of the Ascended Masters. Ride a 19 km mountain in five stages. Chain tricks, hoops and grinds to change the colour of your violet-fire trail, and finish on a giant ramp that launches you into the sun.

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
| **Tight carve** (sharp turn, sheds speed) | Q / E, or Shift + A/D | LB / RB on the ground |
| Tuck / frontflip in air | W or ↑ | Stick up / RT |
| **Brake** (on the ground) / backflip in air | S or ↓ | Stick down / LT |
| Ollie, pop off rails | Space | A |
| Grabs in the air (Indy, Melon, Method) | J K L / Shift | X (Indy), B (Melon), LB (Method), RB (Indy) |
| Violet Flame boost (meter full) | F | Y |
| Lives: 5 or ∞ | ✦ Lives button (start or pause screen) | — |
| Pause · controls · start over (while paused) | P / Esc · Controls button · R | Start · Y · Back/Select |
| Camera (Chase / Far / Close / High) | C or the 🎥 button | Stick click (R3/L3) |
| Music on/off · sound effects on/off | N · M (or the 🎵 / 🔊 buttons) | Back/Select (music) |

## How it plays

- **Combos.** Tricks, hoops and grinds raise the multiplier. The fire trail changes through five tiers: Violet Spark, Violet Flame, Amethyst Blaze, Transmutation and Ascension. Your combo banks into your score once you've been on the snow for 3 full seconds in a row. Scoring on the ground doesn't reset that count; only a real jump, a grind or a crash does.
- **Violet Flame boost.** Combo moves fill the meter. When it is full, it stays full until you use it, and while it waits the meter glows and a button prompt flashes. The boost gives 7 seconds of extra speed (up to 90 km/h over the stage limit) and double points, and you burn through trees instead of crashing into them.
- **The course.** It is the same fixed, seeded course every run. It curves more, gets steeper and fills with more obstacles as you descend. Along the way are steep walls ("Amethyst Wall"), cliff drops ("Leap of Faith") and rollers. Top speed rises stage by stage: 120, 165, 210, 255, then 300 km/h in the final stage. The Violet Flame boost breaks the limit by up to 90 km/h, then eases back down when it ends.
- **Lives.** You have five. Every wipeout costs one, and at zero you start over. Switch to infinite lives with the ✦ Lives button on the start or pause screen (no lives bonus at the finish).
- **The ending.** The run funnels into a giant ramp that launches you into the violet sun, and **YOU WIN**.

## Credits

- Game code: generated with Claude.
- Engine: [three.js](https://threejs.org) (MIT), loaded from jsDelivr.
- Music: *The Blue Danube*, Op. 314 (Johann Strauss II), performed by Das Orchester Tsumugi / Takashi Inoue, live at Fukuoka Symphony Hall, 10 March 2024. Recording courtesy of [www.classicals.de](https://www.classicals.de), licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). The file in `music/blue-danube.mp3` is unmodified (renamed only).
