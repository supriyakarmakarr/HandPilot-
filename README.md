# HandPilot-
AI-powered gesture-controlled presentation system using OpenCV, MediaPipe, and PyAutoGUI.
# Gesture Control Presenter ðŸŽ®ðŸ–ï¸

Control your Google Slides presentations using hand gestures through your laptop camera using Computer Vision and AI.

This project uses:

* OpenCV
* MediaPipe
* PyAutoGUI

to detect hand gestures and convert them into presentation controls like:

* Next Slide
* Previous Slide
* Start Presentation
* Exit Presentation

---

# ðŸš€ Features

âœ… Control Google Slides using gestures
âœ… Real-time hand tracking using AI
âœ… Works directly from laptop webcam
âœ… No additional hardware required
âœ… Beginner-friendly AI + Computer Vision project

---

# ðŸ§  Gesture Controls

| Gesture          | Action          |
| ---------------- | --------------- |
| âœ‹ Open Palm      | Next Slide      |
| ðŸ¤Ÿ Three Fingers | Previous Slide  |
| âœŒï¸ Two Fingers   | Start Slideshow |
| âœŠ Fist           | Exit Slideshow  |

---

# ðŸ› ï¸ Technologies Used

* Python
* OpenCV
* MediaPipe
* PyAutoGUI

---

# ðŸ“¦ Installation

## Step 0 - Ensure Python is installed

For Linux and Mac system, please use `python3` instead of `python` in the commands below </br>

Check if python is installed and available in your system PATH on VSCode Terminal (Terminal â†’ New Terminal):
```bash
python -V
```

---
## Step 1 â€” Download the code

```bash
https://github.com/supriyakarmakarr/HandPilot-
```

---

## Step 2 â€” Install Dependencies

```bash
python -m pip install --break-system-packages -r requirements.txt
```

## Step 3 â€” Download Hand Landmarker Model

```bash
python setup_models.py
```

---

# â–¶ï¸ Run the App

```bash
python main.py
```

---

# Close the application

Press Ctrl+C in terminal to close the application

---


# ðŸ’» macOS Permission Setup

For keyboard control to work on macOS:

Go to:

System Settings â†’ Privacy & Security

Enable permissions for:

* Accessibility
* Input Monitoring

Allow access for:

* Terminal
  OR
* VS Code
  OR
* PyCharm

Without these permissions, the app cannot control Google Slides.

---

# ðŸŽ¯ How to Use

1. Open Google Slides in Chrome
2. Start slideshow mode
3. Run the Python application
4. Show gestures in front of webcam
5. Control slides hands-free

---

# ðŸ“‚ Project Structure

```bash
gesture-control/
â”‚
â”œâ”€â”€ .gitignore
â”œâ”€â”€ main.py
â”œâ”€â”€ README.md
â”œâ”€â”€ requirements.txt
â”œâ”€â”€ setup_models.py
â””â”€â”€ models/
    â””â”€â”€ hand_landmarker.task
```

---

# ðŸ“œ requirements.txt

```txt
mediapipe==0.10.35
opencv-python>=4.8.0
pyautogui>=0.9.54
```

---

# ðŸ§© How It Works

The application:

1. Captures webcam feed using OpenCV
2. Detects hand landmarks using MediaPipe
3. Identifies finger positions
4. Maps gestures to keyboard shortcuts
5. Uses PyAutoGUI to control Google Slides

---

# ðŸ”® Future Improvements

* Swipe gesture recognition
* Gesture-based laser pointer
* Volume control
* Zoom gestures
* AI-powered custom gesture training
* Multi-hand support

---

# ðŸŽ“ Learning Outcomes

This project helps students understand:

* Computer Vision
* AI-based gesture recognition
* Human Computer Interaction (HCI)
* Real-time webcam processing
* Automation using Python

---

# ðŸ“¸ Demo Idea

Use this project during:

* AI Workshops
* Hackathons
* College Tech Fests
* Computer Vision Sessions
* Smart Classroom Demonstrations

---

# âš ï¸ Notes

* Ensure good lighting conditions
* Keep hand visible to webcam
* Avoid cluttered backgrounds for better detection
* Works best at moderate camera distance

---

# Live MediaPipe 
![MediaPipe Hand Tracking Demo](https://google-ai-edge.github.io/mediapipe-samples-web/#/vision/hand_landmarker)
![Google AI Media Pipe] (https://ai.google.dev/edge/mediapipe/solutions/guide)

---

# ðŸ‘¨â€ðŸ’» Built With AI + Computer Vision

A futuristic interaction system powered by hand tracking and real-time gesture recognition.
