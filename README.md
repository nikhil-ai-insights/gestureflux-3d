# ✨ GestureFlux 3D

> An AI-powered 3D particle visualizer that translates real-time hand gestures into immersive motion and sound.


---

## 🚀 Overview

**GestureFlux 3D** is an interactive web experience where users control complex particle systems using natural hand movements.

By combining **MediaPipe's real-time hand tracking** with **Three.js rendering**, the project builds a bridge between physical gestures and generative digital art — transforming motion into visuals and sound.

This project explores **Natural User Interfaces (NUI)** as an intuitive alternative to traditional mouse and keyboard interaction.

---

## ❓ Problem Statement

Traditional digital art tools rely on mouse and keyboard inputs, which often feel indirect and disconnected.

GestureFlux 3D investigates whether AI-powered hand tracking can create a more **expressive, immersive, and natural** way to interact with 3D generative systems.

---

## 🧠 Dataset

The project uses the **MediaPipe Hand Landmarker** pre-trained model, which:

- Detects **21 3D hand landmarks**
- Works in real-time via standard webcam
- Requires **no custom dataset collection**

This enables fast prototyping and low-latency interaction.

---

## 🛠️ Tools & Technologies

| Category | Technology |
|---|---|
| Language | TypeScript |
| 3D Engine | Three.js |
| AI Framework | MediaPipe (Google AI Studio) |
| Build Tool | Vite |
| Deployment | Netlify |
| Sound Engine | Web Audio API (Custom SoundEngine) |

---

## ⚙️ Architecture & Methods

### ✋ Hand Tracking — `HandTracker.ts`

- Captures webcam frames
- Extracts 21 hand landmarks
- Streams real-time positional data

### 🌌 Particle Physics — `ParticleEngine.ts`

- Maps specific landmarks (e.g., thumb, index) to dynamic force fields
- Uses vector math to simulate attraction, repulsion, and flow
- Optimized batching for high particle counts

### 🤏 Gesture Logic

Custom gesture detection calculates:

- **Pinch** → Distance between thumb and index finger
- **Open Palm** → Spread detection across landmarks

These gestures control particle scaling, expansion, and field intensity.

### 🔊 Audio Mapping — `SoundEngine.ts`

- Modulates frequency based on particle density and velocity magnitude
- Creates synchronized audiovisual feedback
- Uses Web Audio API for low-latency synthesis

---

## 📊 Key Insights

**⚡ Low Latency** — MediaPipe enables sub-30ms tracking, critical for real-time creative interaction.

**🎧 Multisensory Feedback** — Visual feedback feels significantly more immersive when paired with synchronized audio modulation.

**🚀 Performance Optimization** — Particle batching in Three.js achieves a stable 60 FPS with 20k+ particles.

---

## 🧪 How To Run Locally

**1. Clone the repository**

```bash
git clone https://github.com/your-username/gesture-flux-3d.git
cd gesture-flux-3d
```

**2. Install dependencies**

```bash
npm install
```

**3. Start development server**

```bash
npm run dev
```

**4. Open in browser**

Visit `http://localhost:5173` and allow camera access when prompted.

---

## 🌍 Deployment

The project is optimized for deployment on **Netlify**.

```bash
npm run build
```

Upload the generated `/dist` folder to Netlify.

---

## 🎯 Results & Conclusion

GestureFlux 3D demonstrates that:

- AI-driven hand tracking can effectively replace traditional input methods
- Natural gestures can control complex generative systems
- Real-time math, motion, and sound can merge into a seamless interactive flow

The result is a lag-free, expressive environment where technology disappears and interaction feels instinctive.

---

## 🔮 Future Improvements

- Multi-hand interaction
- Gesture recording and playback
- Preset visual themes
- VR/WebXR integration
- MIDI export from gesture-driven sound

---

## 📄 License

**MIT License** — feel free to use, modify, and build upon it.
