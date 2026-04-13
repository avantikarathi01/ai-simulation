# ✦ Particle Gestures

An interactive 3D particle simulation controlled by real-time hand gestures via your webcam — built with Three.js and MediaPipe Hands. No frameworks, no build tools, just one HTML file.

---

## What It Does

Your hand becomes the controller. The app reads your webcam feed, detects hand landmarks in real time, and maps gestures to particle behaviors — expanding, collapsing, color-shifting, and switching between 8 stunning 3D shapes.

---

## Features

- 🖐 **Real-time hand gesture recognition** via MediaPipe Hands
- ✨ **5,000 animated particles** rendered with Three.js (WebGL)
- 🔮 **8 particle shapes** — Sphere, Heart, Flower, Saturn, Fireworks, DNA, Galaxy, Wave
- 🎨 **Per-shape color palettes** with pinch-triggered hue cycling
- 🖱 **Mouse fallback** — drag to orbit, scroll to zoom
- 📷 **Live hand skeleton overlay** drawn on a mini webcam preview
- ⚡ **Zero dependencies to install** — runs directly in the browser

---

## Gesture Controls

| Gesture | Action |
|---|---|
| ✋ Open hand | Expand particles |
| ✊ Fist | Collapse particles |
| 🤏 Pinch | Cycle colors |
| ☝ Point up | Switch to next shape |
| ↔ Move hand | Rotate the scene |
| 🖱 Mouse drag | Orbit camera |
| 🖱 Scroll wheel | Zoom in / out |

---

## Technologies Used

| Technology | Purpose |
|---|---|
| [Three.js r128](https://threejs.org/) | 3D WebGL rendering |
| [MediaPipe Hands](https://google.github.io/mediapipe/solutions/hands) | Real-time hand landmark detection |
| [MediaPipe Camera Utils](https://www.npmjs.com/package/@mediapipe/camera_utils) | Webcam frame capture |
| HTML5 Canvas API | Hand skeleton overlay |
| Google Fonts (Space Mono, Playfair Display) | UI typography |

> All libraries are loaded via CDN — no npm install required.

---

## How to Run

### Option 1 — Open directly (simplest)

```bash
# Just open the file in your browser
# Double-click index.html  OR  drag it into Chrome/Edge/Firefox
```

> ⚠️ Some browsers block camera access for `file://` URLs. Use Option 2 if your camera doesn't start.

### Option 2 — Local server (recommended)

**Using VS Code Live Server:**
1. Install the [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
2. Right-click `index.html` → **Open with Live Server**

**Using Python:**
```bash
# Python 3
python -m http.server 8080

# Then open: http://localhost:8080
```

**Using Node.js:**
```bash
npx serve .
# Then open the URL shown in the terminal
```

### First Run
1. Allow camera access when the browser prompts
2. Hold your hand in front of the webcam
3. Try the gestures listed above
4. Click the shape buttons in the top-left to switch shapes manually

---

## Screenshots

> 📸 Screenshots coming soon — drop images in `assets/screenshots/` and update below.

| Sphere | Heart | Galaxy |
|---|---|---|
| ![Sphere](assets/screenshots/sphere.png) | ![Heart](assets/screenshots/heart.png) | ![Galaxy](assets/screenshots/galaxy.png) |

---

## Project Structure

```
particle-gesture-lab/
├── index.html          # Entire app — HTML, CSS, and JS in one file
├── README.md
├── .gitignore
└── assets/
    └── screenshots/    # Add your screenshots here
```

---

## Future Improvements

- [ ] Add touch/mobile gesture support
- [ ] Support two-hand detection for more gesture combinations
- [ ] Add audio reactivity (mic input drives particle energy)
- [ ] Export current particle frame as PNG
- [ ] Add more shapes (torus, cube, text)
- [ ] Settings panel for particle count and speed
- [ ] PWA support for offline use

---

## Browser Support

| Browser | Status |
|---|---|
| Chrome 90+ | ✅ Fully supported |
| Edge 90+ | ✅ Fully supported |
| Firefox 88+ | ✅ Supported |
| Safari 15+ | ⚠️ Camera may need HTTPS |

---

## License

MIT — free to use, modify, and share.
