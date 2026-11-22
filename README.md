# Rasengan Remake

A Rasengan that appears above your palm and follows your hand through the webcam. No effect videos: each style has its own surface, drawn in code from the anime and wrapped on a sphere, with sparks, embers and blades generated live around it.

Inspired by vietnh1009/Naruto, rebuilt from scratch with a procedural engine, so new chakra natures are just new surface data.

Live demo: https://rasengan-remake.vercel.app/

## Styles

- **Classic**: a blue sphere of tangled energy filaments, white, pale blue and gold threads crisscrossing over a bright core.
- **Wind Rasenshuriken**: a bright wind sphere pulled in tight, inside a wide disc of wind cloud drawn from the anime frames, dense at the heart and wispy at the rim, with four blade swirls of denser cloud inside it, fine particles shimmering over it, wind streaks circling and mist at the rim. Charge it with a fist and release, and the disc flares wide.
- **Magnet Rasenshuriken**: a deep blue sphere covered in hundreds of small dark tomoe seals, black orbs circling it, inside a blue wing disc with the seals printed on the disc itself.
- **Lava Rasenshuriken**: a bright molten sphere with embers and smoke, inside a wing disc that runs white hot at the core through orange to deep red at the tips.

## Controls

- Open palm: the sphere fades in above your palm and follows your hand.
- Fist: charge it. The sphere compresses, spins faster, and glows harder.
- Open your hand after a charge: release. The energy pulses out, widest in the Rasenshuriken styles.
- Keys 1 to 4 or the buttons at the bottom: switch style.
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
