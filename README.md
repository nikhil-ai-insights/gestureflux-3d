![image alt](https://github.com/nikhil-ai-insights/gestureflux-3d/blob/65387a8b42c5ee7d0c5500d0d8f7ce51ecbb621b/GestureFlux%203D.png)
# ✨ GestureFlux 3D

> An AI-powered real-time 3D particle visualizer that transforms natural hand gestures into immersive motion and generative sound.

🌍 **[Live Demo]
(https://gestureflux.netlify.app/)**

---

## 🌌 Overview

GestureFlux 3D is an interactive web-based generative art system that allows users to control complex 3D particle simulations using real-time hand gestures.

Built using MediaPipe's AI hand tracking and the Three.js rendering engine, the project bridges physical motion and digital expression. Users interact without mouse or keyboard — only natural gestures.

The result is a fluid, immersive experience where motion, math, physics, and sound merge seamlessly in the browser.

---

## ❓ Problem Statement

Traditional digital creative tools rely on indirect input systems such as mouse and keyboard — often feeling disconnected from the user's natural movement.

GestureFlux 3D explores:

- Can AI-powered hand tracking replace traditional input?
- Can natural gestures control complex generative systems?
- Can interaction feel more instinctive and immersive?

The goal is to design a **Natural User Interface (NUI)** where interaction feels intuitive and frictionless.

---

## 🧠 Dataset

This project uses the **MediaPipe Hand Landmarker** pre-trained model.

- Detects 21 real-time 3D hand landmarks
- Works via standard webcam
- No custom dataset collection required
- Sub-30ms tracking latency

All processing runs directly in the browser — no server-side data storage.

---

## 🛠️ Tools and Technologies

| Category      | Technology                   |
|---------------|------------------------------|
| Language      | TypeScript                   |
| 3D Engine     | Three.js                     |
| AI Framework  | MediaPipe (Google AI Studio) |
| Build Tool    | Vite                         |
| Deployment    | Netlify                      |
| Audio Engine  | Web Audio API                |
| Rendering     | WebGL                        |

---

## ⚙️ Methods

### ✋ Hand Tracking
- Webcam frames captured in real-time
- 21 landmark coordinates extracted per frame
- Landmark vectors streamed continuously to the particle engine

### 🌌 Particle Physics Engine
- Custom force-field system with attraction & repulsion mechanics
- Landmark-driven vector mapping
- Optimized GPU batching
- Stable 60 FPS with 20k+ particles

### 🤏 Gesture Detection
- Pinch detection via thumb-index distance
- Open palm detection via landmark spread analysis
- Gesture-based modulation of particle scale, field intensity, and expansion force

### 🔊 Audio Mapping
- Web Audio API synthesis
- Frequency mapped to particle velocity
- Density-based sound modulation
- Real-time audiovisual synchronization

---

## 📊 Key Insights

**⚡ Real-Time Responsiveness** — Low latency tracking (<30ms) is critical for immersive interaction.

**🎧 Multisensory Feedback** — Combining synchronized audio with visual motion significantly enhances user engagement.

**🚀 Performance Optimization** — Batched particle updates, efficient vector math, and minimal object allocation in the animation loop maintain stable 60 FPS on modern browsers.

**🧠 Natural Interaction Design** — Hand gestures feel significantly more expressive compared to traditional mouse-based control.

---

## 🧪 How to Run This Project

**1️⃣ Clone the Repository**

```bash
git clone https://github.com/your-username/gesture-flux-3d.git
cd gesture-flux-3d
```

**2️⃣ Install Dependencies**

```bash
npm install
```

**3️⃣ Start Development Server**

```bash
npm run dev
```

**4️⃣ Open in Browser**

Visit `http://localhost:5173` and allow camera access when prompted.

---

## 🎯 Results and Conclusion

GestureFlux 3D demonstrates that:

- AI-driven hand tracking can effectively replace traditional input systems
- Natural gestures can control complex generative particle environments
- Real-time physics, motion, and sound can merge into a unified interactive experience

The system achieves low-latency gesture tracking, stable high particle counts (20k+), seamless audiovisual synchronization, and smooth 60 FPS rendering.

GestureFlux 3D represents a step toward the future of natural user interfaces — where technology becomes invisible and interaction feels instinctive.
