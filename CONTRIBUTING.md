# 🤝 Contributing to GestureFlux 3D

First of all, thank you for considering contributing to GestureFlux 3D 🚀  
This project explores AI-driven hand tracking and generative 3D systems — and contributions are always welcome!

Whether you're fixing bugs, improving performance, adding features, or enhancing documentation — your help matters.

---

## 📌 Code of Conduct

Please be respectful and constructive in all discussions. We aim to maintain:

- A positive learning environment
- Clear communication
- Helpful code reviews
- Inclusive collaboration

Har contributor ka respect zaroori hai 🙌

---

## 🛠️ Ways You Can Contribute

### 🐛 Bug Fixes
- Improve tracking stability
- Fix rendering glitches
- Resolve performance bottlenecks

### ✨ Feature Improvements
- Multi-hand interaction
- New gesture detection logic
- Advanced particle behaviors
- WebXR / VR integration
- MIDI export support

### 🎨 UI / UX Enhancements
- Better onboarding experience
- Improved responsiveness
- Visual themes and presets

### 📚 Documentation
- Improve README clarity
- Add architecture diagrams
- Add usage examples

---

## 🚀 Getting Started

**1️⃣ Fork the Repository**

Click **Fork** on GitHub.

**2️⃣ Clone Your Fork**

```bash
git clone https://github.com/your-username/gesture-flux-3d.git
cd gesture-flux-3d
```

**3️⃣ Install Dependencies**

```bash
npm install
```

**4️⃣ Start Development Server**

```bash
npm run dev
```

Visit `http://localhost:5173` and allow camera access when prompted.

---

## 🌿 Branching Strategy

Never push directly to `main`. Follow this branch naming convention:

| Type        | Branch Name Example              |
|-------------|----------------------------------|
| Feature     | `feature/multi-hand-support`     |
| Bug Fix     | `fix/particle-glitch`            |
| Improvement | `improve/performance-batching`   |
| Docs        | `docs/update-readme`             |

---

## 🧪 Development Guidelines

### ✋ Hand Tracking
- Keep tracking logic modular inside `HandTracker.ts`
- Avoid blocking the render loop
- Maintain low latency

### 🌌 Particle Engine
- Optimize GPU batching
- Avoid unnecessary object creation per frame
- Maintain stable 60 FPS

### 🔊 Sound Engine
- Keep audio latency minimal
- Use efficient Web Audio nodes
- Avoid memory leaks in audio graph

### 📏 Code Style
- Use TypeScript strict mode
- Follow consistent naming conventions
- Use descriptive variable names
- Add comments for complex math logic
- Keep functions small and modular

```ts
// Calculate pinch distance between thumb and index
const pinchDistance = calculateDistance(thumbTip, indexTip);
```

---

## 📝 Commit Message Format

```
type: short description
```

**Examples:**

```
feat: add multi-hand tracking support
fix: resolve particle flickering issue
docs: update architecture explanation
perf: optimize particle batching
```

---

## 🔍 Pull Request Guidelines

Before submitting a PR:

- ✅ Ensure the project builds successfully
- ✅ Test in Chrome (latest version recommended)
- ✅ Verify no performance regression
- ✅ Add a clear description of changes
- ✅ Add screenshots/GIF if UI-related

**PR Description Template:**

```markdown
## What does this PR do?
Short explanation.

## Why is this change needed?
Context or issue reference.

## Screenshots (if applicable)
Attach visuals.
```

---

## 🧠 Performance First

GestureFlux 3D focuses heavily on real-time responsiveness, low latency interaction, and smooth 60 FPS rendering. If adding a feature:

- Benchmark performance impact
- Avoid heavy computations inside the animation loop

---

## 💡 Ideas for Advanced Contributors

Want to push the project further? Consider:

- Implementing WebXR support
- Adding physics-based GPU particles
- Adding gesture recording + playback
- Adding ML-based gesture classification
- Creating preset creative modes

---

## 🐞 Reporting Issues

When reporting a bug, please include:

- Browser version
- OS
- Steps to reproduce
- Expected behavior
- Screenshots (if possible)

Clear reports = faster fixes 🚀

---

## 🌍 Community & Discussions

Feel free to open:

- Feature proposals
- Optimization discussions
- Creative experiments
- Architectural improvements

Innovation is welcome 💫

---

## 📄 License

By contributing, you agree that your contributions will be licensed under the **MIT License**.

---

## 🙌 Final Note

GestureFlux 3D is an exploration of AI, generative art, natural interaction, and real-time systems. Your contribution helps push the boundary between human motion and digital expression.

**Let's build the future of interaction together 🚀✨**
