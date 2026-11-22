# Rasengan Remake

A Rasengan that lives in your palm, generated live with particles. No effect videos: 9,000 particles churn on a sphere that tracks your hand through the webcam and scales with your palm.

Inspired by vietnh1009/Naruto, rebuilt from scratch with a procedural engine, so new chakra natures are just new style data.

Live demo: coming with the first deploy.

## Styles

- **Classic**: the wind blue Rasengan, white hot core and a blue swirl disc.
- **Magnet Release**: deep blue chakra threaded with dark seal swirls, with black orbs circling the sphere.
- **Lava Release**: a molten surface with dark crust flecks, hard flicker, embers that fly off and fall back, and a pale smoke cloud behind the sphere.
- **Rasenshuriken**: a tight white hot core with four curved blades of particles spinning around it. Charge it with a fist and release, and the blades flare wide.

## Controls

- Open palm: hold the sphere.
- Fist: charge it. The sphere compresses, spins faster, and glows harder.
- Open your hand after a charge: release. The energy pulses out, widest in Rasenshuriken style.
- Keys 1, 2, 3, 4 or the buttons at the bottom: switch style.
- Take your hand away: the sphere stays where you left it. Show your palm again to pick it up.
- No camera yet? Demo mode follows your mouse until the first hand appears.

## Run it locally

Open `index.html` in a browser and allow the camera, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Tech

Three.js r128 for the particle engine, MediaPipe Hands for tracking. One static file, no build step, nothing to install.

## License

MIT
