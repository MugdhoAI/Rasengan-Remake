# Rasengan Remake

A Rasengan that lives in your palm, generated live with particles. No effect videos: 9,000 particles churn on a sphere that tracks your hand through the webcam and scales with your palm.

Inspired by vietnh1009/Naruto, rebuilt from scratch with a procedural engine, so new chakra natures are just new style data.

Live demo: coming with the first deploy.

## Styles

- **Classic**: the wind blue Rasengan, white hot core and a blue swirl disc.
- **Magnet Release**: deep blue chakra threaded with dark seal swirls, with black orbs circling the sphere.
- **Lava Release**: a molten surface with dark crust flecks, hard flicker, and embers that fly off and fall back.

## Controls

- Open palm: hold the sphere.
- Fist: charge it. The sphere compresses, spins faster, and glows harder.
- Keys 1, 2, 3 or the buttons at the bottom: switch style.
- No camera? Demo mode follows your mouse.

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
