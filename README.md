![image alt](https://github.com/nikhil-ai-insights/gestureflux-3d/blob/65387a8b42c5ee7d0c5500d0d8f7ce51ecbb621b/GestureFlux%203D.png)
# GestureFlux 3D: Turn gestures into motion

GestureFlux 3D is a high-performance, real-time interactive 3D particle system controlled entirely by hand gestures through your webcam. Built with **React**, **Three.js (@react-three/fiber)**, and **Google MediaPipe**, it creates an immersive experience where you "weave" light and sound.

## ✨ Features

- **Gesture Control**: Real-time hand tracking detects pinch, palm expansion, and spatial movement.
- **Dynamic 3D Particles**: Choose between multiple geometric templates:
  - 🪐 **Saturn**: A planetary sphere with orbiting rings.
  - ❤️ **Hearts**: A romantic, swirling heart formation.
  - 🌸 **Flowers**: Intricate rose-curve petal patterns.
  - 🎆 **Fireworks**: Randomly dispersed explosive structures.
- **Generative Sound Engine**: A Web Audio API backend that synthesizes sound based on your hand tension (pinch) and energy (expansion).
- **Glassmorphism UI**: A sleek, translucent control panel for real-time customization.

## 🖐️ Gesture Controls

| Gesture | Action | Audio Response |
| :--- | :--- | :--- |
| **Pinch** | Change scale of the structure | Shifts oscillator frequency (tension) |
| **Open Palm** | Expand / Explode particles | Increases filter cutoff (brightness/energy) |
| **Move Hand** | Translate structure in 3D space | Adjusts ambient hum |

## 🚀 Getting Started

This project is designed to run in modern browsers using ES Modules.

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/gesture-flux-3d.git
   ```

2. **Run a local server**:
   Because this uses Camera permissions and ESM imports, you must serve it via `localhost`. You can use any static server:
   ```bash
   npx serve .
   ```

3. **Open the browser**:
   Navigate to `http://localhost:3000` (or the port specified by your server).

## 🛠️ Tech Stack

- **React 19**: UI and State Management.
- **Three.js & React Three Fiber**: 3D rendering and particle math.
- **MediaPipe Hands**: Real-time computer vision for hand tracking.
- **Web Audio API**: Generative synthesizer logic.
- **Tailwind CSS**: Modern UI styling.

## 📜 License

This project is licensed under the MIT License. Feel free to use it for your own cosmic experiments!
