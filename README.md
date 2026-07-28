# <h1 align="center">🌌 Particle Sphere</h1>

<p align="center">
<b>A real-time hand-controlled 3D particle simulation built with Three.js and MediaPipe.</b><br>
Control a <b>3000-particle interactive sphere</b> using nothing but your hands—no mouse, no keyboard, no installation required.
</p>

<p align="center">
<a href="https://3d-particle.netlify.app"><img src="https://img.shields.io/badge/🚀%20Live-Demo-00C7B7?style=for-the-badge"></a>
<a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge"></a>
</p>

<p align="center">
<img alt="Three.js" src="https://img.shields.io/badge/Three.js-r160-black?style=for-the-badge&logo=three.js">
<img alt="MediaPipe" src="https://img.shields.io/badge/MediaPipe-Hands-00897B?style=for-the-badge&logo=google">
<img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
<img alt="Netlify" src="https://img.shields.io/badge/Hosted-Netlify-00C7B7?style=for-the-badge&logo=netlify">
<img alt="Build" src="https://img.shields.io/badge/Build-None-8A8D92?style=for-the-badge">
</p>

---

# 🎥 Demo

> **Live Website**

https://3d-particle.netlify.app

---

# 📸 Preview

The best way to showcase this project is with a **GIF** at the top followed by screenshots.

```
assets/
│
├── demo.gif
├── idle.png
├── charge.png
├── burst.png
├── morph.png
└── colors.png
```

Then use:

<p align="center">
<img src="assets/demo.gif" width="90%" alt="Particle Sphere Demo">
</p>

---

### Screenshots

<p align="center">
<img src="assets/idle.png" width="48%">
<img src="assets/charge.png" width="48%">
</p>

<p align="center">
<img src="assets/burst.png" width="48%">
<img src="assets/morph.png" width="48%">
</p>

<p align="center">
<img src="assets/colors.png" width="70%">
</p>

---

# ✨ Features

## 🖐️ Gesture Controls

Control the entire scene using natural hand gestures detected through your webcam.

| Gesture                 | Action                      |
| ----------------------- | --------------------------- |
| ✋ Move one hand         | Rotate and move the sphere  |
| 🤏 Pinch & Hold         | Charge an energy ring       |
| ✨ Release pinch         | Explode the particle sphere |
| 🙌 Spread both hands    | Increase sphere size        |
| 🤲 Bring hands together | Shrink sphere               |
| ✊ Hold a fist (~0.8s)   | Morph geometry              |
| ☝️ Show 0–5 fingers     | Change particle colors      |

---

## 🌟 Visual Effects

* 3000 animated particles
* Motion trails
* Dynamic glow
* Smooth particle interpolation
* Morphing geometry
* Energy charging animation
* Explosion physics
* Webcam background mode
* PNG screenshot capture
* Responsive full-screen rendering

---

## ⌨️ Keyboard & Mouse Controls

Even without a webcam, the experience remains fully interactive.

| Key         | Action          |
| ----------- | --------------- |
| Drag Mouse  | Rotate sphere   |
| Mouse Wheel | Scale sphere    |
| Space       | Burst particles |
| M           | Morph geometry  |
| 0–5         | Change colors   |

---

# ⚙️ Built With

* **Three.js** – GPU accelerated particle rendering
* **MediaPipe Hands** – Real-time hand landmark detection
* **HTML5**
* **CSS3**
* **Vanilla JavaScript**

No frameworks.

No build tools.

No npm dependencies.

Everything lives inside a **single HTML file**.

---

# 🚀 Getting Started

Clone the repository

```bash
git clone https://github.com/yourusername/particle-sphere.git

cd particle-sphere
```

Serve locally

```bash
python3 -m http.server 8000
```

Open

```
http://localhost:8000
```

You can also use:

* Live Server (VS Code)
* npx serve
* Any static web server

> Camera permissions require HTTPS or localhost.

---

# 🌐 Deployment

Since this project is entirely static, deployment is effortless.

Supported platforms:

* Netlify
* Vercel
* GitHub Pages
* Cloudflare Pages

Simply upload the project folder or connect your Git repository.

---

# 📂 Project Structure

```
Particle-Sphere/

│
├── particle-sphere.html
├── README.md
│
└── assets/
    ├── demo.gif
    ├── idle.png
    ├── charge.png
    ├── burst.png
    ├── morph.png
    └── colors.png
```

---

# ⚡ Performance

* ~3000 GPU-rendered particles
* Real-time hand tracking
* 60 FPS on most modern desktops
* Runs entirely on-device
* No data leaves your computer

---

# 🌍 Browser Support

✔ Chrome

✔ Edge

✔ Firefox

✔ Brave

WebGL and `getUserMedia()` support are required.

---

# 💡 Future Improvements

* Multi-user interaction
* Gesture recording
* VR/WebXR support
* More particle presets
* Physics-based interactions
* Mobile optimization

---

# 📜 License

Released under the **MIT License**.

Feel free to use, modify, and build upon this project.

---

<p align="center">

Made with ❤️ using Three.js + MediaPipe

</p>

