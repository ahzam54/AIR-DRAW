# ✋ AIR DRAW

> Draw in the air with your finger. No mouse. No stylus. Just your hand.

AIR DRAW is a real-time hand gesture drawing app powered by Computer Vision. It uses your webcam and MediaPipe hand tracking to turn your index finger into a brush — letting you paint, erase, and switch tools entirely through hand gestures.

---

## 🎬 Demo

> **[🚀 Try it live on Hugging Face Spaces](https://huggingface.co/spaces/Ahzan001/AIR-DRAW)**

<!-- Add a demo GIF here -->
<!-- Tip: Record a short screen capture, convert to GIF using ezgif.com, upload to repo and link below -->

![AIR DRAW Demo](demo.gif)

> *Replace `demo.gif` with your own screen recording. Even 10 seconds works great.*

---

## ✨ Features

| Gesture | Action |
|---|---|
| ☝️ Index finger up | Draw |
| ✌️ Peace sign | Erase |
| ✋ Open palm (hold) | Open tool menu |
| ✊ Fist | Close menu |

- 🎨 Multiple brush colors via on-screen palette
- 🖌️ Bezier curve smoothing for natural strokes
- ✨ Particle effects on every brush stroke
- 📱 Mobile support with touch fallback
- 💡 Auto brightness boost in low light
- 🔁 Undo support
- 🖥️ Works entirely in the browser — no install needed

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 Canvas | Drawing surface |
| CSS3 | Neon cyberpunk UI |
| Vanilla JavaScript | App logic & gesture handling |
| [MediaPipe Hands](https://mediapipe.dev/) | Real-time hand landmark detection |
| WebRTC / getUserMedia | Camera access |

Zero dependencies. No Python. No backend. Pure browser tech.

---

## 🚀 Run Locally

No install required. Just open the file:

```bash
git clone https://github.com/ahzam54/AIR-DRAW.git
cd AIR-DRAW
# Open index.html in your browser
open index.html   # macOS
start index.html  # Windows
```

> ⚠️ Camera access requires a browser that supports `getUserMedia`. Works best in Chrome or Edge.

---

## 🧠 How It Works

```
Webcam feed
    ↓
MediaPipe Hands (21 hand landmarks detected per frame)
    ↓
Gesture classifier (index up = DRAW, peace = ERASE, open palm = MENU)
    ↓
Exponential moving average smoothing (removes jitter)
    ↓
Bezier curve renderer on HTML5 Canvas
    ↓
Particle system + HUD update
```

The gesture recognition runs at **30 FPS on desktop**, **15 FPS on mobile** — fast enough for smooth, natural drawing.

---

## 📁 Project Structure

```
AIR-DRAW/
├── index.html       # Entire app — single file
└── README.md
```

---

## 🔭 What's Next

- [ ] AI-powered drawing recognition (show shape → Claude names it)
- [ ] Save drawing as PNG
- [ ] Multi-hand support
- [ ] Shape snap mode (draws perfect circles, rectangles)
- [ ] Prompt Engineering integration — describe your drawing to AI

---

## 👨‍💻 Built By

**Ahzan Imam** — Final-year Engineering Student at IEM Kolkata
Passionate about Computer Vision, Prompt Engineering, and building AI that feels human.

🔗 [LinkedIn](https://www.linkedin.com/in/ahzan-imam/) • 🤗 [Hugging Face](https://huggingface.co/Ahzan001) • 💻 [GitHub](https://github.com/ahzam54)

---

## 📄 License

MIT License — free to use, modify, and share.

---

*Built with Computer Vision + a lot of ☕*
