# Rasengan Remake

A Rasengan that appears above your palm and follows your hand through the webcam. No effect videos: each style has its own surface, drawn in code from the anime and wrapped on a sphere, with sparks, embers and blades generated live around it.

Inspired by vietnh1009/Naruto, rebuilt from scratch with a procedural engine, so new chakra natures are just new surface data.

Live demo: https://rasengan-remake.vercel.app/

## Styles

- **Classic**: pale blue with white wind streaks flowing across the surface, and a swirl disc around the ball.
- **Magnet Release**: deep blue covered in dark tomoe seal clusters, with black orbs circling the sphere.
- **Lava Release**: a molten surface of orange flows, white hot spots and dark crust cracks, embers flying off, and a pale smoke cloud behind the sphere.
- **Rasenshuriken**: a bright wind sphere pulled in tight, with four curved blades spinning around it. Charge it with a fist and release, and the blades flare wide.

## Controls

- Open palm: the sphere fades in above your palm and follows your hand.
- Fist: charge it. The sphere compresses, spins faster, and glows harder.
- Open your hand after a charge: release. The energy pulses out, widest in Rasenshuriken style.
- Keys 1, 2, 3, 4 or the buttons at the bottom: switch style.
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
