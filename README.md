# Rasengan Remake

A Rasengan that appears above your palm and follows your hand through the webcam. No effect videos: each style has its own surface, drawn in code from the anime and wrapped on a sphere, with sparks, embers and blades generated live around it.

Inspired by vietnh1009/Naruto, rebuilt from scratch with a procedural engine, so new chakra natures are just new surface data.

Live demo: https://rasengan-remake.vercel.app/

## Styles

- **Classic**: a blue sphere of tangled energy filaments, white, pale blue and gold threads crisscrossing over a bright core.
- **Magnet Release**: deep blue covered in hundreds of small dark tomoe seals, with black orbs circling the sphere.
- **Lava Release**: a bright molten surface of orange flows and white hot areas with thin dark crust, embers flying off, and a pale smoke cloud behind the sphere.
- **Wind Rasenshuriken**: a bright wind sphere pulled in tight, inside a flat, dense disc of 9,000 tiny particles with four blade arms. Charge it with a fist and release, and the disc flares wide.
- **Magnet Rasenshuriken**: the Magnet sphere inside a blue wing disc flecked with dark seals.
- **Lava Rasenshuriken**: the Lava sphere inside a wing disc that runs white hot at the core through orange to deep red at the tips, with embers and smoke.

## Controls

- Open palm: the sphere fades in above your palm and follows your hand.
- Fist: charge it. The sphere compresses, spins faster, and glows harder.
- Open your hand after a charge: release. The energy pulses out, widest in the Rasenshuriken styles.
- Keys 1 to 6 or the buttons at the bottom: switch style.
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
