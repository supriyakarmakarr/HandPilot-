<div align="center">

  <!-- Header Banner with 🖐️ Hand & Glowing Gradient -->
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=1,12,24,30&height=250&section=header&text=🖐️%20HandPilot&fontSize=70&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=AI-Powered%20Gesture-Controlled%20Presentation%20System&descFontSize=22&descAlignY=58&descAlign=50" width="100%" alt="HandPilot Header" />

  <!-- Animated Waving Hand & Subtitle -->
  <h2>
    <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="36" alt="Waving Hand" />
    <span>Control Your Slides Hands-Free with Hand Gestures!</span>
    <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="36" alt="Waving Hand" />
  </h2>

  <!-- Animated Typing Subtitle -->
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=18&duration=3000&pause=1000&color=00F5D4&center=true&vCenter=true&width=600&lines=Touchless+Slide+Navigation+Powered+by+AI;Real-Time+MediaPipe+Hand+Landmark+Tracking;Control+Google+Slides+%26+PPT+with+Webcam;Zero+External+Hardware+Required" alt="Typing SVG" />
  </a>

  <br/><br/>

  <!-- Badges -->
  <p align="center">
    <img src="https://img.shields.io/badge/Python-3.9%2B-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
    <img src="https://img.shields.io/badge/OpenCV-4.8%2B-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" alt="OpenCV" />
    <img src="https://img.shields.io/badge/MediaPipe-0.10%2B-00C0FF?style=for-the-badge&logo=google&logoColor=white" alt="MediaPipe" />
    <img src="https://img.shields.io/badge/PyAutoGUI-Automation-FF6F00?style=for-the-badge&logo=autohotkey&logoColor=white" alt="PyAutoGUI" />
    <img src="https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey?style=for-the-badge&logo=linux&logoColor=black" alt="Cross-Platform" />
  </p>

  <img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="650" alt="Divider Animation" />

</div>

---

## ⚡ Overview

**HandPilot** allows you to control **Google Slides, PowerPoint, Keynote, Canva, and PDFs** using simple hand gestures in front of your laptop webcam. No clickers, remotes, or extra hardware required!

---

## 🎮 Gesture Controls

<div align="center">

| Gesture | Visual | Action | Shortcut | Details |
| :---: | :---: | :---: | :---: | :--- |
| **Four Fingers (4)** | 4️⃣ ✋ | **Next Slide** | `Right Arrow (→)` | 4 Fingers up (Thumb tucked in) |
| **Three Fingers (3)** | 3️⃣ 🤟 | **Previous Slide** | `Left Arrow (←)` | 3 Fingers up (Index, Middle, Ring) |
| **Two Fingers (2)** | 2️⃣ ✌️ | **Start Slideshow** | `F5` / `Cmd+Enter` | 2 Fingers up (Peace / V-Sign) |
| **Closed Fist (0)** | 0️⃣ ✊ | **Exit Slideshow** | `Escape (Esc)` | All fingers closed into a fist |

<br/>

<!-- MediaPipe 21 Hand Landmarks Points Diagram -->
<img src="https://developers.google.com/static/mediapipe/images/solutions/hand-landmarks.png" width="440" alt="MediaPipe 21 Landmarks Diagram" />

<p><em>MediaPipe 21 3D Hand Landmark Points used for tracking & gesture classification</em></p>

</div>

---

## 🚀 Quick Setup & Run (3 Simple Steps)

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/supriyakarmakarr/HandPilot-.git
cd HandPilot-
```

### 2️⃣ Install Dependencies & AI Model
```bash
# Install required libraries
pip install -r requirements.txt

# Download MediaPipe task model
python setup_models.py
```

### 3️⃣ Start HandPilot!
```bash
python main.py
```

> 🛑 **To Stop:** Press **`q`** on the camera window or **`Ctrl + C`** in terminal.

---

## 🎯 How to Use

1. Open your presentation (**Google Slides / PowerPoint / PDF**) in full screen.
2. Run `python main.py` in terminal.
3. Show gestures in front of your webcam (**0.5m – 1.5m distance**) to control slides hands-free!

<details>
<summary><b>🍎 macOS Users Note (Click to Expand)</b></summary>

<br/>

Enable **Accessibility** & **Input Monitoring** for your terminal app under:
**System Settings** → **Privacy & Security** → **Accessibility / Input Monitoring**.

</details>

---

## 📂 Project Structure

```bash
HandPilot-/
├── 📁 models/              # MediaPipe AI landmarker model
├── 📄 main.py              # Main application (Camera + Gestures + Keystrokes)
├── 📄 setup_models.py      # AI Model auto-downloader
├── 📄 requirements.txt     # Dependencies
└── 📄 README.md            # Documentation
```

---

## 🔮 Roadmap

- [x] Real-time 21-point hand tracking
- [x] Slide navigation (Next, Prev, Start, Exit)
- [ ] 👆 Virtual Laser Pointer (Fingertip on-screen pointer)
- [ ] 💨 Swipe Gestures (Air swipe transitions)
- [ ] 🔊 Air Volume Control (Wrist rotation)

---

## 🌟 Support

Agar yeh project pasand aaye toh ek ⭐️ **Star** zaroor dein!

<div align="center">

  <a href="https://github.com/supriyakarmakarr/HandPilot-">
    <img src="https://img.shields.io/github/stars/supriyakarmakarr/HandPilot-?style=social" alt="Stars" />
  </a>
  <a href="https://github.com/supriyakarmakarr/HandPilot-/fork">
    <img src="https://img.shields.io/github/forks/supriyakarmakarr/HandPilot-?style=social" alt="Forks" />
  </a>

  <br/><br/>

  <!-- Footer Banner -->
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=1,12,24,30&height=120&section=footer" width="100%" alt="HandPilot Footer" />

  <p>Crafted with ❤️ by <a href="https://github.com/supriyakarmakarr"><b>Supriya Karmakar</b></a></p>

</div>
