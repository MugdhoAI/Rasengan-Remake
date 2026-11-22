# Wind Style Rasen Shuriken

![Wind Style Rasen Shuriken](docs/assets/wind-style-rasen-shuriken-hero.svg?v=1)

A Rasengan that appears above your palm and follows your hand through the webcam. No effect videos: every style has its own surface, drawn in code from the anime and wrapped on a sphere, with sparks, embers and blades generated live around it.

**Live demo: https://wind-style-rasen-shuriken.vercel.app/**

Inspired by vietnh1009/Naruto, rebuilt from scratch with a procedural engine, so new chakra natures are just new surface data.

## Styles

| Key | Style | What you see |
| --- | --- | --- |
| 1 | Classic | A blue sphere of tangled energy filaments, white, pale blue and gold threads over a bright core |
| 2 | Wind Rasenshuriken | A bright wind sphere pulled in tight, inside a wide disc of wind cloud drawn from the anime frames, four soft cloud blades whose tips hook in the spin, wind streaks and rim mist |
| 3 | Magnet Rasenshuriken | A bright blue sphere tiled with the real seal pattern, a dark ring with a dot inside it, black orbs with violet rims on a tilted ring, inside a clean blue cloud disc |
| 4 | Lava Rasenshuriken | A bright molten sphere with embers and smoke, inside a cloud disc of bent pale blades edged with flame, over a ring of fire clouds |
| 5 | Dual, Magnet + Lava | Both hands at once: Magnet Rasenshuriken in your left hand, Lava Rasenshuriken in your right, each with its own disc and its own charge |

## Controls

- Open palm: the sphere fades in above your palm and follows your hand.
- Fist: charge it. The sphere compresses, spins faster, and glows harder.
- Open your hand after a charge: release. The energy pulses out, widest in the Rasenshuriken styles.
- Keys 1 to 5 or the buttons at the bottom: switch style.
- A second hand mirrors the effect in every style, and each hand charges on its own fist.
- Take your hand away: the sphere fades out, like the original. Show your palm to bring it back.

## How it works

- Each style surface is a canvas texture drawn in code at load: filament fields for wind, the ring and dot seal grid for Magnet, layered molten blobs for Lava.
- The wing disc is a drawn cloud, soft puffs with denser cloud along four curved blade spines, because particles alone read as noise and plain gradients wash out.
- Two complete effect instances run at once, one per tracked hand, which is what makes Dual mode possible.
- Hand tracking is MediaPipe Hands, up to two hands, and the effect exists only while a palm is on screen.

## Run it locally

Open `index.html` in a browser and allow the camera, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Tech

Three.js r128 for the sphere, its drawn surfaces and the live particles. MediaPipe Hands for tracking. One static file, no build step, nothing to install.

## License

MIT
