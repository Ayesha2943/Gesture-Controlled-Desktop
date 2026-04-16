# 🖐️ Gesture Controlled Cursor using Computer Vision

A real-time gesture-based cursor control system built using Python, OpenCV, and MediaPipe. This project enables users to control the mouse cursor using hand gestures captured via a webcam.

---

## 🚀 Project Overview

This project implements a real-time gesture-controlled cursor system using computer vision techniques. It leverages **MediaPipe’s pre-trained hand tracking model (TensorFlow Lite backend)** to detect hand landmarks in real time.

The system maps hand gestures such as finger movements and pinches into mouse actions like cursor movement, clicking, and scrolling.

---

## ⚠️ Important Note

This project is still under development and not fully polished. It requires further improvements in:

* Gesture accuracy
* Stability
* Performance

---

## 🧠 Core Concept

The system works in the following steps:

1. Capture video from the webcam using OpenCV
2. Detect hand landmarks using MediaPipe
3. Interpret gestures based on landmark positions
4. Map gestures to mouse actions using PyAutoGUI

---

## 🛠️ Tech Stack

### 🐍 Python

Core programming language used for implementation

### 📷 OpenCV

* Captures video from webcam
* Processes image frames
* Converts frames to RGB for MediaPipe
* Displays output window with FPS

### ✋ MediaPipe (TensorFlow Lite Backend)

* Provides pre-trained hand tracking model
* Detects **21 hand landmarks** in real time
* Enables gesture recognition without training a custom AI model

### 🖱️ PyAutoGUI

Used to control system mouse:

* Cursor movement
* Left click
* Right click
* Scrolling

### 🔢 NumPy

Used for interpolation and coordinate mapping

### 📐 Math Library

Used for calculating distances between landmarks

### ⏱️ Time Module

Used for FPS calculation and performance tracking

---

## ⚙️ Features

* 🖱️ Cursor movement using index finger
* 👆 Left click using thumb + index finger pinch
* 👉 Right click using index + middle finger pinch
* 🔄 Scroll using two-finger vertical movement
* 🎯 Smooth cursor movement using interpolation
* 📊 FPS display for performance monitoring
* 📷 Real-time hand tracking

---

## 🧾 Gesture Mapping

| Gesture                            | Action      |
| ---------------------------------- | ----------- |
| Index finger up                    | Move cursor |
| Thumb + Index pinch                | Left click  |
| Index + Middle pinch               | Right click |
| Two fingers up (vertical movement) | Scroll      |

---

## 🧪 How It Works (Technical)

* MediaPipe detects **21 hand landmarks**

* Important landmarks used:

  * Index finger tip → (8)
  * Thumb tip → (4)
  * Middle finger tip → (12)

* Gesture detection is based on distance between landmarks:

```python
distance = hypot(p2.x - p1.x, p2.y - p1.y)
```

* Based on distance thresholds, gestures are classified and mapped to actions.

---

## ▶️ Installation

```bash
git clone https://github.com/your-username/gesture-controlled-cursor.git
cd gesture-controlled-cursor
pip install -r requirements.txt
```

---

## ▶️ Usage

```bash
python main.py
```

Make sure your webcam is enabled. Perform gestures in front of the camera to control your cursor.

---

## 🔮 Future Improvements

* Improve gesture recognition accuracy
* Reduce latency and improve performance
* Add customizable gesture controls
* Support multi-hand interactions

---

## 🙋‍♀️ Author

Ayesha
B.E. in AI & Data Science

---

## ⭐ Contributing

Feel free to fork this repository and contribute by submitting a pull request.

---

## 📜 License

This project is open-source and available under the MIT License.

