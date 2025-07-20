# 💪 CV-Based Shoulder Press Exercise Analysis

## 🧠 Overview

This project is a **Computer Vision-based real-time exercise analysis tool** that helps users perform **shoulder press exercises** with proper posture and form. It uses **OpenCV** and **MediaPipe** to detect and analyze body movements, providing **live posture feedback**, **rep counting**, and **calorie estimation**. Users can choose between a **live webcam stream** or **pre-recorded videos** for analysis.

> The tool features a **graphical user interface (GUI)** built with **Tkinter**, along with engaging visuals, background music, goal setting, and a performance summary screen.

---

## 🏋️‍♂️ Key Features

- 📸 **Live Camera or Recorded Video Mode**
- 🧍‍♂️ Real-time **pose estimation** using **MediaPipe**
- 🔄 **Shoulder and elbow angle** calculation to validate posture
- ✅ **Correct/Incorrect posture classification**
- 🔢 **Repetition counter** and **set tracking**
- ⏱️ **Timer** for workout duration
- 🔥 **Calories burned** estimation based on user’s weight and time
- 📊 **Result Summary** with total reps, duration, and calories burned
- 🎯 **Set personal workout goals**
- 🎵 Optional **background music**
- 🖼️ Visual progress bars and animations

---

## 📁 Project Structure

```
📦 Shoulder_Press_Analysis/
├── Shoulder_Press_Analysis.py   # Main application script
├── 📁 assets/                   # Contains all images and icons (e.g., pic.png, im.png, camera.png)
├── 📁 sound/                    # Background music files for the session
```

---

## ⚙️ Technologies Used

| Purpose               | Library / Tool        |
|----------------------|-----------------------|
| Pose Estimation       | MediaPipe             |
| Video Processing      | OpenCV                |
| GUI                   | Tkinter + PIL         |
| Audio Playback        | Pygame                |
| Math & Utilities      | NumPy, Math, Threading|

---

## 🚀 How to Run

### 🖥️ Requirements

Make sure the following Python libraries are installed:

```bash
pip install opencv-python mediapipe numpy pygame pillow
```

### ▶️ Run the App

```bash
python Shoulder_Press_Analysis.py
```

> ⚠️ Make sure you have a working webcam and all image/audio assets are in place in the expected directories (`assets/`, `sound/`).

---

## 📊 Output Summary

At the end of the workout, the app displays:

- 🎯 Whether the target was achieved
- ⏰ Total duration of the session
- 🔁 Total reps completed
- 🔥 Calories burned (based on MET formula and user weight)

---

## 👨‍💻 Developed By

**Ali Sajid** & **Noor Sultan**  
Mechatronics and Control Engineering  
University of Engineering and Technology, Lahore  
**Under supervision of:** Prof. Ahsan Naeem

---

## 🌱 Future Enhancements

- Add more exercises (e.g., squats, lunges, push-ups)
- Posture correction suggestions
- Cloud storage for session data
- Integration with fitness wearables

---

