# 🚀 NavAid: Assistive Navigation System for the Visually Impaired

NavAid is a real-time assistive system designed to support visually impaired users by detecting surrounding objects and providing voice-guided alerts. The system runs on a Raspberry Pi, processes live camera input, and delivers immediate feedback to improve situational awareness.

📘 New to Raspberry Pi? See the detailed setup guide: [Raspberry Pi Setup](BEGINNER_GUIDE.md)

---

## 🎯 Overview

* Detects ~91 object classes in real time
* Provides **audio feedback** for nearby obstacles
* Designed as a **portable embedded system**
* Focuses on **practical usability and real-time performance**

This project emphasizes building a working assistive solution rather than purely optimizing accuracy metrics.

---

## ⚙️ Key Features

* 🎥 Real-time object detection using YOLO
* 🔊 Voice alerts using text-to-speech (pyttsx3)
* 📏 Distance-aware notifications for nearby objects
* ⚡ Lightweight deployment on Raspberry Pi
* 🌐 Works offline (no cloud dependency)

---

## 🧠 System Workflow

Camera Input → Object Detection (YOLO) → Distance Estimation → Voice Alert

The system continuously captures frames, detects objects, estimates proximity, and generates corresponding audio alerts.

---

## 🛠️ Tech Stack

* **Programming:** Python
* **Computer Vision:** OpenCV, YOLO
* **Hardware:** Raspberry Pi
* **Audio Output:** pyttsx3 (Text-to-Speech)

---

## 🔧 Setup (Quick Start)

```
git clone https://github.com/SyedSahil80328/NavAid.git
mv NavAid blindhelper
cd blindhelper
sudo apt-get update
sudo apt-get install python3-dev python3-pip python3-opencv python3-numpy espeak
pip install -r requirements.txt
python IASDriver.py
```

> Ensure the camera is connected and enabled on the Raspberry Pi before running.

---

## ▶️ Usage

1. Power on Raspberry Pi with camera attached
2. Run the main script
3. System starts detecting objects and giving voice alerts
4. Press `q` to stop execution

---

## 📊 Observations & Limitations

* Performs well on **known objects in controlled environments**
* Struggles with **unseen objects or cluttered scenes**
* GPS-based navigation was explored but not implemented due to hardware limitations

---

## 👤 My Contribution

* Configured Raspberry Pi and hardware setup
* Integrated object detection with voice alert pipeline
* Worked on real-time processing and testing
* Documented workflow and structured implementation

---

## 🔗 Future Improvements

* Improve generalization for unseen objects
* Optimize detection speed and latency
* Integrate reliable navigation support (GPS or alternatives)
