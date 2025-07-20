# Shoulder Press Exercise Analysis using Computer Vision

---

## Table of Contents
- [Overview](#overview)  
- [Features](#features)  
- [Technologies Used](#technologies-used)  
- [How It Works](#how-it-works)  
- [Project Structure](#project-structure)  
- [Getting Started](#getting-started)  
- [Running the Application](#running-the-application)  
- [Future Enhancements](#future-enhancements)  
- [License](#license)  

---

## Overview

This project is a **Computer Vision-based Shoulder Press Exercise Analyzer** developed in Python. It uses your webcam or pre-recorded videos to monitor your shoulder press exercise form in real time. It provides instant feedback on posture, counts repetitions and sets, tracks workout duration, and estimates calories burned. The application includes a gamified and user-friendly graphical interface with visual progress bars and motivational background music to help keep you engaged and motivated throughout your workout.

---

## Features

- **Real-time form correction and posture analysis:** Uses pose detection to analyze joint angles and provide immediate feedback.  
- **Repetition and set counting:** Automatically counts valid reps and sets based on form correctness.  
- **Custom workout goal setup:** Users can set desired numbers of reps, sets, or workout duration.  
- **Calorie estimation:** Estimates calories burned based on workout time and exercise intensity (using MET calculations).  
- **Visual feedback:** Progress bars and angle measurements are displayed to help users understand their performance.  
- **Workout timer:** Tracks the duration of each session.  
- **Result summary dashboard:** Shows total workout time, calories burned, reps completed, and goal achievements at session end.  
- **Supports both live camera and pre-recorded video input:** Flexible input options for different use cases.

---

## Technologies Used

### 1. OpenCV  
OpenCV is used for video capturing (from webcam or video files), frame processing, and displaying annotated video frames with posture visuals in real time.

### 2. Mediapipe  
Mediapipe provides highly accurate pose detection and extracts 33 body landmark coordinates. This project uses landmarks like shoulder, elbow, and wrist to calculate joint angles critical for shoulder press form analysis.

### 3. Tkinter (GUI)  
Tkinter is Python’s built-in graphical user interface toolkit. It creates the user interface window displaying the live video feed, workout controls, progress bars, posture status messages, and session summaries.

### 4. PIL (Pillow)  
The Pillow library is used to convert OpenCV’s BGR frames into an image format compatible with Tkinter’s canvas for smooth and real-time GUI rendering.

### 5. Pygame  
Pygame is employed to play background music during workout sessions, enhancing the user’s engagement and motivation.

---

## How It Works

1. **Pose Detection:**  
   The application uses Mediapipe’s pose estimation to detect and track body landmarks in each video frame.

2. **Angle Calculation:**  
   Using the coordinates of shoulder, elbow, and wrist landmarks, it calculates elbow and shoulder joint angles with geometric formulas.

3. **Form Analysis:**  
   The joint angles are compared against predefined ideal ranges for a correct shoulder press form. When angles meet the criteria, the program counts a repetition and displays a "CORRECT" status in green. Incorrect form prompts corrective feedback.

4. **Progress Monitoring:**  
   The GUI shows progress bars indicating how close the user is to completing reps, sets, or workout duration goals. A timer tracks the total session time.

5. **Result Summary:**  
   Once the workout finishes or the goal is reached, a summary screen shows total time spent, calories burned (calculated based on the duration and MET values for shoulder press), and overall performance statistics.

---

## Project Structure

├── main.py # Main script to run the application
├── assets/ # Folder containing images, icons, and audio files
│ ├── pic.png # Sample image assets
│ ├── browse_back.png # UI navigation icons
│ └── background_music.mp3 # Background music file for workouts
├── README.md # Project documentation (this file)
└── requirements.txt # List of required Python libraries
