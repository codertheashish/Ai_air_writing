# Ai_air_writing
AI Virtual Air Writing with Colors & Eraser is a real-time, AI-powered system that lets users draw in the air using just their index finger. Leveraging MediaPipe’s hand tracking model and OpenCV, it tracks hand movements, converts them into digital strokes on a virtual canvas, and records the session as a video. Users can switch between multiple pen colors, erase strokes, and clear the canvas — all without touching a screen. This project demonstrates a seamless combination of computer vision, machine learning, and interactive creative tools.

---

# ✋ **AI Virtual Air Writing (OpenCV + MediaPipe + AI Hand Tracking)**

A real-time **AI-powered Air Writing system** that lets you **draw in the air using your index finger** — no touch, no stylus.
Powered by **MediaPipe’s machine-learning hand tracking** and **OpenCV**, this project turns your webcam into an AI gesture-controlled drawing tool.

---

## ✨ **Features**

* 🎨 Multiple pen colors (Red, Green, Blue)
* ✏ Finger-based Air Drawing
* 🧽 Eraser Tool with thick brush
* 🧼 Clear Canvas instantly
* 🤖 AI Hand Tracking (21 keypoints)
* 📹 Automatic MP4 recording of session
* 🚀 Works on Windows / macOS / Linux

---

## 🎮 **Controls**

| Key           | Action                             |
| ------------- | ---------------------------------- |
| **W**         | Toggle Drawing Mode (ON/OFF)       |
| **E**         | Toggle Eraser Mode                 |
| **C**         | Clear Canvas                       |
| **1 / 2 / 3** | Switch Colors (Red / Green / Blue) |
| **ESC**       | Exit Program                       |

---

## 🛠 **Tech Stack**

* **Python 3.x**
* **OpenCV** → Video capture, drawing, video recording
* **MediaPipe Hands** → ML-based hand landmark detection
* **NumPy**

---

## 📦 **Installation**

### 1️⃣ Clone the Repository

```bash
https://github.com/your-username/ai_air_writing.git
```

### 2️⃣ Install Dependencies

```bash
pip install opencv-python mediapipe
```

---

## ▶️ **How to Run**

Make sure your webcam is connected, then run:

```bash
python ai_air_writing.py
```

Your terminal will show a live webcam feed with drawing overlay.

---

## 📁 **Output**

All sessions are automatically saved as:

```
air_writing_color_tools1.mp4
```

---

## 🤖 **How the AI Works**

1. MediaPipe detects hands using a pretrained ML model.
2. Index finger tip (**landmark #8**) is tracked.
3. Finger movement is converted into strokes on a **transparent canvas**.
4. Canvas + camera feed are merged with:

```python
cv2.addWeighted(frame, 0.6, canvas, 0.8, 0)
```

5. AI tracking ensures smooth, stable drawing even during fast movements.

---

## 🌟 **Future Enhancements**

* Gesture-based writing (pinch-to-draw, palm-to-erase)
* AI-based handwriting smoothing
* Shape prediction (circle, square, arrow)
* Multi-hand support
* Convert drawings to text using CNN/RNN
* On-screen GUI buttons

---

## 📜 **License**

Released under the **MIT License** — free to use and modify.

---

## 👨‍💻 **Author**

**Ashish Kumar Prajapati**

---
