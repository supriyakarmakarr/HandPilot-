<div align="center">

  <!-- Header Banner -->
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=1,12,24,30&height=260&section=header&text=🖐️%20HandPilot&fontSize=70&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Next-Gen%20AI%20Gesture-Controlled%20Presentation%20System&descFontSize=22&descAlignY=58&descAlign=50" width="100%" alt="HandPilot Header" />

  <!-- Animated Typing Subtitle -->
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=3000&pause=1000&color=00F5D4&center=true&vCenter=true&width=650&lines=Touchless+Slide+Navigation+Powered+by+AI;Real-Time+MediaPipe+21-Point+Hand+Landmark+Tracking;Control+Google+Slides+%26+PowerPoint+with+Webcam;Zero+External+Sensors+or+Hardware+Required" alt="Typing SVG" />
  </a>

  <br/><br/>

  <!-- Badges -->
  <p align="center">
    <img src="https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
    <img src="https://img.shields.io/badge/OpenCV-4.8+-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" alt="OpenCV" />
    <img src="https://img.shields.io/badge/MediaPipe-0.10+-00C0FF?style=for-the-badge&logo=google&logoColor=white" alt="MediaPipe" />
    <img src="https://img.shields.io/badge/PyAutoGUI-Automation-FF6F00?style=for-the-badge&logo=autohotkey&logoColor=white" alt="PyAutoGUI" />
    <img src="https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey?style=for-the-badge&logo=linux&logoColor=black" alt="Cross-Platform" />
  </p>

  <p align="center">
    <a href="#-overview">Overview</a> •
    <a href="#-gesture-control-matrix">Gestures</a> •
    <a href="#-key-features">Features</a> •
    <a href="#-system-architecture--workflow">Architecture</a> •
    <a href="#-installation--setup">Installation</a> •
    <a href="#-future-roadmap">Roadmap</a>
  </p>

  <img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="700" alt="Divider Animation" />

</div>

---

## ⚡ Overview

**HandPilot** is an intelligent touchless presentation system powered by Computer Vision & Artificial Intelligence. Using your laptop’s built-in webcam, **HandPilot** tracks 21 distinct 3D landmarks on your hand in real time via **Google MediaPipe**, classifies custom hand gestures through spatial geometry, and seamlessly translates them into native keyboard keystrokes using **PyAutoGUI** to control **Google Slides, PowerPoint, Keynote, Canva, or PDF decks**.

> 💡 **Why HandPilot?** Say goodbye to clickers, dongles, and being stuck next to your laptop during presentations. Just wave, point, or gesture naturally from anywhere in your camera's field of view!

---

## 🎮 Gesture Control Matrix

<div align="center">

| Gesture | Visual | Action | Triggered Shortcut | Description |
| :---: | :---: | :---: | :---: | :--- |
| **Open Palm** | 🖐️ | **Next Slide** | `Right Arrow` / `Space` | All 5 fingers extended facing camera |
| **Three Fingers** | 🤟 / 🖖 | **Previous Slide** | `Left Arrow` / `Backspace` | Index, Middle, & Ring fingers raised |
| **Victory / Peace** | ✌️ | **Start Slideshow** | `F5` / `Ctrl+F5` / `Cmd+Enter` | Index & Middle fingers extended |
| **Closed Fist** | ✊ | **Exit Slideshow** | `Escape (Esc)` | All fingers curled into a tight fist |

</div>

<br/>

<div align="center">
  <img src="https://developers.google.com/static/mediapipe/images/solutions/hand-landmarks.png" width="460" alt="MediaPipe 21 Landmarks Diagram" />
  <p><em>MediaPipe 21 3D Hand Landmark Coordinates utilized by HandPilot</em></p>
</div>

---

## 🚀 Key Features

<table>
  <tr>
    <td width="50%">
      <h3>🔮 Real-Time Hand Tracking</h3>
      <p>Tracks full 3D hand spatial landmarks with ultra-low latency (~30+ FPS) using Google's optimized ML pipelines.</p>
    </td>
    <td width="50%">
      <h3>🎯 Zero Additional Hardware</h3>
      <p>Runs directly using standard 720p/1080p built-in laptop webcams or external USB cameras. No sensors needed.</p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h3>🛡️ Smart Gesture Debouncing</h3>
      <p>Built-in cooldown frames and state-locking mechanisms prevent accidental double-skips and flickering triggers.</p>
    </td>
    <td width="50%">
      <h3>🌐 Universal Deck Compatibility</h3>
      <p>Works effortlessly with <b>Google Slides, Microsoft PowerPoint, Keynote, Canva, Notion Presentations, and PDF Readers</b>.</p>
    </td>
  </tr>
</table>

---

## 🛠️ System Architecture & Workflow

```mermaid
graph LR
    A[📹 Webcam Video Stream] --> B[🖼️ OpenCV Frame Processing]
    B --> C[🤖 MediaPipe 21-Point Landmark Detection]
    C --> D[📐 Finger State & Spatial Geometry Engine]
    D --> E{🎯 Gesture Classifier}
    E -->|Open Palm 🖐️| F1[➡️ Next Slide]
    E -->|Three Fingers 🤟| F2[⬅️ Previous Slide]
    E -->|Two Fingers ✌️| F3[▶️ Start Slideshow]
    E -->|Fist ✊| F4[⏹️ Exit Slideshow]
    F1 & F2 & F3 & F4 --> G[⌨️ PyAutoGUI Virtual Keystroke]
    G --> H[🖥️ Google Slides / PPT / Keynote]
