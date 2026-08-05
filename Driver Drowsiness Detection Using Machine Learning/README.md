<div align="center">

# 🚗 Driver Drowsiness Detection Through Face Mesh

### Real-time facial monitoring · Head-pose analysis · Raspberry Pi alert system

A team academic project designed to detect visible signs of driver fatigue and trigger an audible alert before drowsiness contributes to an accident.

![Python](https://img.shields.io/badge/Python-3.7-3776AB?style=for-the-badge&logo=python&logoColor=white)
![MediaPipe](https://img.shields.io/badge/MediaPipe-Face%20Mesh-00BFA5?style=for-the-badge)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-4-A22846?style=for-the-badge&logo=raspberrypi&logoColor=white)
![Status](https://img.shields.io/badge/Status-Academic%20Prototype-orange?style=for-the-badge)

</div>

---

## Project Summary

Driver fatigue can develop gradually through signs such as prolonged eye closure, yawning, frequent blinking, head nodding and loss of concentration. This project proposes a non-invasive monitoring system that observes the driver through a camera, analyses facial landmarks and head position, classifies the driver as alert or drowsy, and activates an audible warning when drowsiness is detected.

The submitted project report states:

- **97.5% detection accuracy in the straight-face position**
- **Approximately 3 seconds system response time**
- A low-cost embedded design using a **Raspberry Pi 4, webcam and speaker**

These figures should be understood as results reported for the stated prototype conditions, not as proof of performance in every vehicle, lighting condition or driver population.

---

## Problem Statement

How can driver drowsiness be detected in real time under changing head positions and environmental conditions, so that the driver receives an early warning before fatigue contributes to an accident?

---

## How the System Works

```text
Driver's face
     |
     v
Webcam captures live video
     |
     v
Frame preprocessing and face detection
     |
     v
MediaPipe Face Mesh identifies facial landmarks
     |
     v
Head-position and facial-behaviour analysis
     |
     v
Decision: Alert or Drowsy
     |
     +---- Alert ------> Continue monitoring
     |
     +---- Drowsy -----> Sound warning through speaker
```

### Main processing stages

1. **Video capture** — a webcam continuously records the driver's face.
2. **Face and feature detection** — the system locates the face and extracts useful facial information.
3. **Face Mesh analysis** — facial landmarks are used to observe face orientation and movement.
4. **Head-pose tracking** — pitch, yaw and roll help describe whether the head moves up, down, sideways or toward the shoulders.
5. **Drowsiness decision** — patterns such as nodding, extended downward tilt and slow swaying movement are compared with thresholds.
6. **Alert generation** — an audible alarm warns the driver when the system detects a drowsy condition.

---

## Hardware

| Component | Purpose |
|---|---|
| Raspberry Pi 4 | Embedded computer that runs the monitoring logic |
| Webcam | Captures the driver's face in real time |
| Speaker / sound box | Produces the warning alarm |
| HDMI or USB cable | Connects display and peripheral devices |
| Power supply | Powers the Raspberry Pi and connected equipment |
| Connecting wires | Connects the alert hardware |

---

## Software and Methods

- Python 3.7
- Linux
- MediaPipe Face Mesh
- Facial-landmark analysis
- Head-pose estimation
- Threshold-based decision logic
- Real-time camera processing

> Add only libraries that appear in the actual source code. Do not claim OpenCV, TensorFlow, scikit-learn or a trained classifier unless the repository contains evidence that they were used.

---

## System Modules

- Webcam module
- Video-capture module
- Face-detection and feature-extraction module
- Face Mesh algorithm module
- Raspberry Pi module
- Drowsiness-classification or decision module
- Alerting module

---

## Reported Prototype Results

| Metric | Reported result |
|---|---|
| Detection accuracy | 97.5% in the straight-face position |
| Response time | Approximately 3 seconds |
| Alert type | Audible warning |
| Deployment style | Low-cost embedded prototype |

### Accuracy note

A supporting research paper included with the project materials reports up to **99% accuracy for a Random Forest classifier on the NTHUDDD dataset** using eye aspect ratio, mouth aspect ratio and head-pose features. That is a **literature benchmark**, not automatically the measured result of this student prototype. It should only be presented as this project's result if the same experiment, dataset and evaluation were personally reproduced and documented.

---

## Team

This was a team academic project submitted by:

- P. S. N. V. Sri Sai
- B. Chitesh Kumar
- B. Avinash
- P. Ramya

Guided by Dr. A. V. N. Chandra Sekhar, Department of Information Technology, Sasi Institute of Technology and Engineering.

### My Contribution

### My Contribution

This was a four-member academic team project.

My contribution included:

- Participating in the project design and research
- Studying driver-drowsiness indicators and Face Mesh
- Supporting the system architecture and module design
- Contributing to project documentation and presentation
- Participating in testing and evaluation

More detailed source-code attribution will be added after reviewing the original project files.

---

## Repository Structure

```text
driver-drowsiness-detection/
├── README.md
├── requirements.txt
├── .gitignore
├── LICENSE
├── src/
│   └── README.md
├── models/
│   └── README.md
├── assets/
│   └── README.md
├── tests/
│   └── README.md
└── docs/
    ├── PROJECT_OVERVIEW.md
    ├── CLIENT_EXPLANATION.md
    ├── STAR_STORY.md
    └── LIMITATIONS_AND_FUTURE_WORK.md
```

---

## Running the Project

The executable source code was not included in the supplied report files. After adding the real code, replace this section with verified instructions such as:

```bash
python -m venv .venv
```

```bash
# Windows
.venv\Scripts\activate
```

```bash
pip install -r requirements.txt
python src/main.py
```

Do not publish instructions that have not been tested on a clean computer.

---

## Limitations

- The report's accuracy claim is specifically for a straight-face position.
- Camera-based detection can be affected by poor lighting, camera quality and face occlusion.
- Glasses, sunglasses, masks or multiple faces may reduce landmark reliability.
- Fixed thresholds may not work equally well for every person.
- A warning system reduces risk but cannot guarantee accident prevention.
- The project is an academic prototype and is not certified for safety-critical automotive use.

---

## Future Improvements

- Combine eye closure, yawning and head pose instead of depending mainly on head angle.
- Calibrate thresholds for each driver.
- Test during day, night, glare and low-light conditions.
- Evaluate drivers with glasses, sunglasses and different face shapes.
- Measure precision, recall, F1-score and false-alarm rate, not only accuracy.
- Add event logging and a driver/fleet safety dashboard.
- Use infrared or low-light cameras.
- Test on a recognised dataset and clearly separate training subjects from test subjects.
- Add privacy controls and process video locally where possible.
- Conduct controlled, ethical validation before any real-world deployment.

---

## Safety and Ethics

This repository is an educational demonstration. It must not be treated as a replacement for adequate sleep, professional medical advice, safe driving practices or certified automotive safety systems.

Do not test the system while driving on public roads. Use recorded videos, a simulator or a stationary vehicle in a controlled environment.

---

## Author Profile

**B. Chitesh Kumar**

- GitHub: [chitesh1207](https://github.com/chitesh1207)
- LinkedIn: [Chitesh Kumar](https://www.linkedin.com/in/chitesh-kumar/)

---

<div align="center">

### Using machine learning and embedded systems to explore safer transportation

</div>
