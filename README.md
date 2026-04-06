# Finger_counter-using-hand-tracking

Hand Gesture Finger Counter using OpenCV & MediaPipe
A real-time computer vision project that detects hand landmarks and counts the number of fingers using your webcam.

Built using:
- OpenCV
- MediaPipe
- Python 🐍

## 📸 Demo Preview
 Features:
- Hand tracking
- Finger counting (0–5)
- Overlay images based on finger count
- FPS counter

## 📂 Project Structure
finger_counter/
│
├── main.py
├── HandTrackingModule.py
├── FingerImages/
│   ├── 1.png
│   ├── 2.png
│   ├── 3.png
│   ├── 4.png
│   ├── 5.png
│   └── 6.png
└── README.md

## ⚙️ How It Works
🔹 Hand Detection
- Uses MediaPipe Hands to detect 21 landmarks per hand
- Implemented in `HandTrackingModule.py`
🔹 Finger Detection Logic
- Thumb → compared using x-axis
- Other fingers → compared using y-axis
🔹 Finger Counting: totalFingers = fingers.count(1)

```python

⚙️ Installation
1. Clone the repository
git clone https://github.com/your-username/finger-counter.git
cd finger-counter
2. Create virtual environment
python -m venv venv
venv\Scripts\activate   # Windows
3. Install dependencies
pip install opencv-python mediapipe


⚠️ Requirements
Python 3.10 / 3.11 recommended
Webcam access
Good lighting for accurate detection

🐞 Common Issues 
cv2 not working → install in correct environment
mediapipe error → use Python 3.10
camera not opening → try cv2.VideoCapture(0)

📸 Output
Live webcam feed
Hand landmarks drawn
Finger count displayed visually

🔮 Future Improvements
🤖 Gesture-based controls (volume, brightness)
🖱️ Virtual mouse
🎮 Game controls using hand gestures
📱 Mobile camera integration








