<h1 align="center"><i>Particle</i> Sphere</h1>
<p align="center"><i>A 3000-point 3D particle sphere you control with your bare hands, in real time, in a single HTML file.</i></p>

<p align="center">
  <a href="https://3d-particle.netlify.app"><strong>→ Live demo</strong></a>
</p>

<p align="center">
  <img alt="Three.js" src="https://img.shields.io/badge/THREE.JS-r160-000000?style=for-the-badge&logo=three.js&logoColor=white">
  <img alt="MediaPipe" src="https://img.shields.io/badge/MEDIAPIPE-HANDS-00897B?style=for-the-badge&logo=google&logoColor=white">
  <img alt="JavaScript" src="https://img.shields.io/badge/JAVASCRIPT-VANILLA-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
  <img alt="No build step" src="https://img.shields.io/badge/BUILD%20STEP-NONE-8A8D92?style=for-the-badge">
  <img alt="Netlify" src="https://img.shields.io/badge/DEPLOYED-NETLIFY-00C7B7?style=for-the-badge&logo=netlify&logoColor=white">
  <img alt="License" src="https://img.shields.io/badge/LICENSE-MIT-8A8D92?style=for-the-badge">
</p>

---

No mouse, no keyboard, no install — pinch to charge and burst the sphere apart, spread two hands to grow it, hold a fist to morph its shape, and count your fingers to shift its color. Everything runs client-side against your webcam.

## Preview

<!-- screenshots go here, e.g.:
<p align="center">
  <img src=<h1 align="center"><i>Particle</i> Sphere</h1>
<p align="center"><i>A 3000-point 3D particle sphere you control with your bare hands, in real time, in a single HTML file.</i></p>

<p align="center">
  <a href="https://3d-particle.netlify.app"><strong>→ Live demo</strong></a>
</p>

<p align="center">
  <img alt="Three.js" src="https://img.shields.io/badge/THREE.JS-r160-000000?style=for-the-badge&logo=three.js&logoColor=white">
  <img alt="MediaPipe" src="https://img.shields.io/badge/MEDIAPIPE-HANDS-00897B?style=for-the-badge&logo=google&logoColor=white">
  <img alt="JavaScript" src="https://img.shields.io/badge/JAVASCRIPT-VANILLA-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
  <img alt="No build step" src="https://img.shields.io/badge/BUILD%20STEP-NONE-8A8D92?style=for-the-badge">
  <img alt="Netlify" src="https://img.shields.io/badge/DEPLOYED-NETLIFY-00C7B7?style=for-the-badge&logo=netlify&logoColor=white">
  <img alt="License" src="https://img.shields.io/badge/LICENSE-MIT-8A8D92?style=for-the-badge">
</p>

---

No mouse, no keyboard, no install — pinch to charge and burst the sphere apart, spread two hands to grow it, hold a fist to morph its shape, and count your fingers to shift its color. Everything runs client-side against your webcam.

## Preview

<!-- screenshots go here, e.g.:
<p align="center">
  <img src="./assets/screenshot-idle.png" alt="Idle sphere state" width="49%">
  <img src="./assets/screenshot-burst.png" alt="Burst / explosion state" width="49%">
</p>
-->

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

There's also a webcam-as-background toggle, a one-click PNG snapshot, an ambient glow that tracks the current color, motion trails, and a full keyboard/mouse fallback (drag to rotate, scroll to scale, `Space` to burst, `M` to morph, `0`–`5` to force a color) for whenever a camera isn't available.

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

It's a static file, so any static host works. This project is deployed on [Netlify](https://www.netlify.com/) at **[3d-particle.netlify.app](https://3d-particle.netlify.app)**:

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

MIT — do whatever you'd like with it.">
  <img src="./assets/screenshot-burst.png" alt="Burst / explosion state" width="49%">
</p>
-->

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

There's also a webcam-as-background toggle, a one-click PNG snapshot, an ambient glow that tracks the current color, motion trails, and a full keyboard/mouse fallback (drag to rotate, scroll to scale, `Space` to burst, `M` to morph, `0`–`5` to force a color) for whenever a camera isn't available.

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

It's a static file, so any static host works. This project is deployed on [Netlify](https://www.netlify.com/) at **[3d-particle.netlify.app](https://3d-particle.netlify.app)**:

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
