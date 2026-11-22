# Wind Style Rasen Shuriken

A Rasengan that appears above your palm and follows your hand through the webcam. No effect videos: each style has its own surface, drawn in code from the anime and wrapped on a sphere, with sparks, embers and blades generated live around it.

Inspired by vietnh1009/Naruto, rebuilt from scratch with a procedural engine, so new chakra natures are just new surface data.

Live demo: https://wind-style-rasen-shuriken.vercel.app/

## Styles

- **Classic**: a blue sphere of tangled energy filaments, white, pale blue and gold threads crisscrossing over a bright core.
- **Wind Rasenshuriken**: a bright wind sphere pulled in tight, inside a wide disc of wind cloud drawn from the anime frames, dense at the heart and wispy at the rim, with four soft cloud blades inside it whose tips hook in the spin, fine particles shimmering over it, wind streaks circling the same way the disc turns and mist at the rim. Charge it with a fist and release, and the disc flares wide.
- **Magnet Rasenshuriken**: a bright blue sphere tiled with the real seal pattern, a dark ring with a dot inside it, copied from the sphere Naruto holds, black orbs with violet rims floating on a tilted ring around the core, inside a clean blue cloud disc. The seals live only on the sphere, never on the wings.
- **Lava Rasenshuriken**: a bright molten sphere with embers and smoke, inside a cloud disc of bent pale blades edged with flame, over a ring of fire clouds.
- **Dual, Magnet + Lava**: the exceptional fifth style, and it uses both hands. Show both palms and the Magnet Rasenshuriken forms in your left hand while the Lava Rasenshuriken forms in your right, each with its own disc, embers, orbs and charge.

## Controls

- Open palm: the sphere fades in above your palm and follows your hand.
- Fist: charge it. The sphere compresses, spins faster, and glows harder.
- Open your hand after a charge: release. The energy pulses out, widest in the Rasenshuriken styles.
- Keys 1 to 5 or the buttons at the bottom: switch style.
- Style 5, Dual: show both hands and hold both natures at once, Magnet in your left hand, Lava in your right. In every style, a second hand mirrors the effect, and each hand charges on its own fist.
- Take your hand away: the sphere fades out, like the original. Show your palm to bring it back.

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
