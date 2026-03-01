# 🔐 Security Policy – GestureFlux 3D

Thank you for helping keep GestureFlux 3D secure 🙌

Security is extremely important for a project that uses real-time webcam access, processes live hand tracking data, and runs browser-based audio & rendering engines. We take responsible disclosure seriously.

---

## 🛡️ Supported Versions

Please ensure you are using the latest version before reporting issues.

| Version              | Supported |
|----------------------|-----------|
| Latest `main` branch | ✅ Yes    |
| Older versions       | ❌ No     |

---

## 🚨 Reporting a Vulnerability

If you discover a security vulnerability, please **DO NOT open a public issue**.

Instead, contact us privately:

- 📧 **Email:** `your-email@example.com`
- **Subject line:** `Security Vulnerability – GestureFlux 3D`

Please include:

- Description of the vulnerability
- Steps to reproduce
- Potential impact
- Screenshots / Proof of Concept (if applicable)
- Your suggested mitigation (optional)

We aim to respond within **48–72 hours**.

---

## 🔎 Scope of Security Concerns

GestureFlux 3D runs entirely in the browser. Security considerations include:

### 🎥 1. Webcam Access

- Uses MediaPipe via browser APIs
- Requires explicit user permission
- No video data is stored or transmitted
- No server-side video processing

If you identify unauthorized camera access, hidden data transmission, or permission bypass behavior — **please report immediately**.

### 🌐 2. Client-Side Rendering & Injection

Potential areas of concern:

- XSS vulnerabilities
- Unsafe DOM manipulation
- Third-party dependency exploits

We follow these practices:

- No unsafe `innerHTML` usage
- Strict TypeScript typing
- Controlled dependency updates

### 🔊 3. Web Audio API Risks

The audio engine runs locally in the browser. We ensure:

- No microphone access
- No audio recording
- No external audio streaming

Only synthesized sound based on gesture data is produced.

### 📦 4. Dependency Security

Project uses TypeScript, Three.js, MediaPipe, and Vite. We recommend running:

```bash
npm audit
```

If you discover a critical dependency vulnerability, please report it privately.

---

## 🔒 Data Privacy Policy

GestureFlux 3D:

- ❌ Does **NOT** collect personal data
- ❌ Does **NOT** store video frames
- ❌ Does **NOT** transmit hand landmark data to any server
- ❌ Does **NOT** use analytics by default

All processing happens **locally in the browser**.

---

## ⚙️ Deployment Security (Netlify)

When deploying:

- Ensure HTTPS is enabled
- Do not expose API keys in client code
- Avoid committing `.env` files
- Keep build output clean

---

## 🧪 Security Best Practices for Contributors

If contributing to this project:

- Never commit secrets or credentials
- Avoid adding remote tracking scripts
- Keep dependencies minimal
- Validate any external input
- Avoid `eval`-like functions
- Follow strict TypeScript rules

---

## ⏳ Disclosure Process

1. Vulnerability reported privately
2. Maintainer acknowledges within 72 hours
3. Issue investigated & patch prepared
4. Responsible disclosure announcement (if necessary)
5. Credit given to reporter (if desired)

---

## 🎯 Out of Scope

The following are **not** considered security issues:

- Browser permission prompts
- Minor performance issues
- Denial of camera access by user
- Expected WebGL limitations
- Client-side inspection of source code

---

## 🙏 Responsible Disclosure

We appreciate security researchers and ethical hackers. Please allow reasonable time to resolve issues before public disclosure.

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 🚀 Final Note

GestureFlux 3D is built around real-time AI, natural interaction, and browser-based performance. Security ensures that innovation remains safe and trustworthy.

**Thank you for helping make GestureFlux 3D secure 🔐✨**
