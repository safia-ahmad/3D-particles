# Particle Sphere

A 3D particle sphere, made of 3000 points, that you control with your bare hands — no mouse, no keyboard, just a webcam. Pinch to charge and burst it apart, spread two hands to grow it, hold a fist to morph its shape, and count your fingers to shift its color.

**[→ Live demo](https://3d-particle.netlify.app)**

Built as a single HTML file. No frameworks, no build step, no backend.

---

## What it does

| Gesture | Effect |
|---|---|
| Move one hand | Sphere follows your palm and rotates with your motion |
| Pinch (thumb + index) and hold | A ring at your fingertips charges up |
| Release the pinch | Sphere explodes into scattered particles, then reforms |
| Spread two hands apart | Sphere grows |
| Bring two hands together | Sphere shrinks |
| Hold a fist (~0.8s) | Sphere morphs shape — sphere → torus → double helix → sphere |
| Show 0–5 fingers | Particle color shifts through a spectrum |

There's also a webcam-as-background toggle, a one-click PNG snapshot, an ambient glow that tracks the current color, and a full keyboard/mouse fallback (drag to rotate, scroll to scale, `Space` to burst, `M` to morph, `0`–`5` to force a color) for whenever a camera isn't available.

## Tech

- **[Three.js](https://threejs.org/)** — WebGL particle rendering
- **[MediaPipe Hands](https://developers.google.com/mediapipe)** — real-time hand landmark tracking, entirely client-side
- Vanilla JS, HTML, CSS — no framework, no bundler, no dependencies to install

Everything lives in one file: `particle-sphere.html`.

## Running it locally

Camera access requires a secure context, so opening the file directly (`file://`) won't work in most browsers. Serve it instead:

```bash
python3 -m http.server 8000
```

then open `http://localhost:8000/particle-sphere.html`.

Any static server works the same way — `npx serve`, VS Code's Live Server, etc.

## Deploying

It's a static file, so any static host works. This project is deployed on [Netlify](https://www.netlify.com/):

```bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>
# drag the folder into https://app.netlify.com/drop
# or connect the repo in the Netlify dashboard for auto-deploys on push
```

GitHub Pages, Vercel, and Cloudflare Pages all work identically — just make sure the site is served over HTTPS (or `localhost`), since browsers block camera access otherwise.

## Browser support

Needs a browser with WebGL and `getUserMedia` support — recent Chrome, Edge, or Firefox on desktop. Performance depends on your GPU and how well your webcam feed lights your hands; try to keep your hand clearly lit and in-frame for the most reliable tracking.

## License

MIT — do whatever you'd like with it.
