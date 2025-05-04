# PoseApp

PoseApp is a simple Android application that removes the background from the live camera feed and overlays a pose estimation skeleton in real time. It uses MediaPipe’s SelfieSegmenter and Pose detection models to isolate the user and analyze their body posture.

---

## Features

- 📸 Real-time camera feed using CameraX
- 🧍‍♂️ Live background removal with MediaPipe SelfieSegmenter
- 🦴 Pose estimation with skeleton overlay (MediaPipe Pose)
- 🧱 Built with Jetpack Compose UI framework
- 🔧 Firebase App Distribution 

---

## Technologies

- Kotlin
- Jetpack Compose
- CameraX
- MediaPipe:
  - `SelfieSegmenter` for background removal
  - `Pose` model for skeletal tracking
- Firebase App Distribution

---

## How It Works

- The app opens a camera preview using CameraX.
- Each frame is processed with MediaPipe to:
  - Segment the person and render them with a transparent or custom background.
  - Detect body keypoints (pose estimation) and draw a skeleton representing the posture.
- The result is a live augmented video stream showing both the person and their pose.

---

## Setup Instructions

### Requirements

- Android Studio (latest stable)
- JDK 17+
- A physical Android device (segmentation may not work properly on emulators)

### To Run

1. Clone this repository
2. Open the `PoseApp/android` folder in Android Studio
3. Plug in your Android device and click "Run"

---

## Folder Overview

```
PoseApp/
├── android/ # Android Studio native app
│ ├── app/ # Source code and layouts
│ └── google-services.json # Firebase config
├── node_modules/ # Auto-generated dependencies
└── README.md
```
