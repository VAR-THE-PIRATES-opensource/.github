# VAR
# 💪 AI Pose Similarity & Push-Up Counter

An interactive real-time pose detection and fitness tracker built using **Kivy**, **OpenCV**, and **TensorFlow Lite**.

This application compares your **real-time camera feed** against reference **pose images** extracted from a video. It uses AI to:
- Detect **key body joints**
- Visualize **pose similarity**
- And count **push-up reps** based on elbow angle movement

---

## 🖼️ Screenshots

| Pose Matching | Push-up Counter |
|---------------|-----------------|
| ![Pose Match](screenshots/pose_comparison.png) | ![Push-up Count](screenshots/pushup_counter.png) |

> 📷 Place your screenshots inside a `screenshots/` folder with matching names.

---

## 🎥 Demo

Watch the working demo in action:

👉 **[Click to Watch Video](video/demo.mp4)**  
_(Place your `.mp4` in a `video/` folder in the repo. GitHub will auto-embed a playable link!)_

Alternatively, upload the demo to YouTube and link it here.

---

## 🚀 Features

- 📸 Real-time webcam feed using OpenCV
- 📊 Pose similarity comparison with reference images
- 🧠 AI model (TFLite) for keypoint detection
- 🔗 Skeletal connections visualization
- 📐 Angle-based push-up detection with count overlay
- 🖥️ Dual screen mode: Pose Viewer & Fitness Tracker

---

## 📁 Project Structure

```plaintext
ai_pos_detection_similarity/
├── RUN.py                       # Main Kivy application
├── thundermore.tflite           # Pose estimation TFLite model
├── outputs/                     # Frames extracted from a video
├── images.png                   # Default fallback image
├── funcalgosearch.py            # Pose angle matching logic
├── checkifsetsaresame.py        # Utility to compare keypoint sets
├── checksiffilepresent.py       # Checks for next available frame
├── turntoframe.py               # Converts video to frames
├── screenshots/                 # Screenshots for README
└── video/                       # MP4 demo clip
