# 🖐️ Gesture Controlled Desktop

A Python-based project that enables users to control their computer system using hand gestures. This system uses computer vision techniques to track hand movements and perform actions like mouse movement, clicking, and volume control without any physical touch.

## 🚀 Features

* Control mouse cursor using hand gestures
* Left click and right click using finger gestures
* Scroll functionality
* Volume control using hand distance
* Real-time hand tracking using webcam
* Works without any external hardware

## 🛠️ Technologies Used

* Python
* OpenCV
* MediaPipe
* PyAutoGUI
* NumPy

## 📌 How It Works

The system captures video input from the webcam and detects hand landmarks using MediaPipe. Based on the position and distance between fingers, different gestures are recognized and mapped to system controls like mouse movement, clicks, and volume adjustment.

## 📂 Project Structure

```
Gesture-Controlled-Desktop/
│── main.py
│── hand_tracking_module.py
│── requirements.txt
│── README.md
```

## ⚙️ Installation

1. Clone the repository:

```
git clone https://github.com/your-username/gesture-controlled-desktop.git
```

2. Navigate to the project folder:

```
cd gesture-controlled-desktop
```

3. Install required libraries:

```
pip install -r requirements.txt
```

## ▶️ Usage

Run the main file:

```
python main.py
```

Make sure your webcam is enabled. Perform hand gestures in front of the camera to control your system.

## 🎯 Applications

* Touchless computer interaction
* Useful for presentations
* Accessibility support
* Human-computer interaction research

## 🔮 Future Improvements

* Add gesture customization
* Improve accuracy in low light conditions
* Add multi-hand support
* Integrate more system controls

## 🙋‍♀️ Author

Ayesha
B.E. in AI & Data Science

## ⭐ Contributing

Feel free to fork this repository and contribute by submitting a pull request.

## 📜 License

This project is open-source and available under the MIT License.
