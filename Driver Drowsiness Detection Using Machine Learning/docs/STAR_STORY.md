# STAR Interview Story

## Complete project STAR answer

### Situation

Road accidents can occur when fatigued drivers lose concentration or experience microsleep. Existing solutions may require body sensors, depend on vehicle data, or become unreliable under changing lighting and head positions. Our team wanted to explore a low-cost, non-invasive system using a camera and embedded computer.

### Task

Our task was to design an academic prototype that could monitor visible driver behaviour in real time, identify a drowsy condition from facial or head-position information, and trigger an audible alert.

### Action

We designed a pipeline in which:

1. A webcam captured live video of the driver.
2. The system located the face and extracted useful facial information.
3. MediaPipe Face Mesh supplied facial landmarks for head-position analysis.
4. Head movement was described through pitch, yaw and roll.
5. Decision thresholds were used to distinguish alert and drowsy behaviour.
6. A Raspberry Pi 4 acted as the embedded processing unit.
7. A speaker produced an audible warning when a drowsy condition was detected.
8. The architecture, modules, hardware and UML workflow were documented in the project report.

Replace this with your personal contribution:
“I was personally responsible for [YOUR TRUE CONTRIBUTION]. One problem I handled was [TRUE PROBLEM], and I solved it by [TRUE ACTION].”

### Result

The project report states that the prototype achieved 97.5% accuracy in the straight-face position and responded in approximately three seconds. The outcome was a low-cost academic architecture capable of monitoring the driver and generating an audible warning.

### Reflection

The most important lesson was that accuracy alone is not enough for a safety system. We must also measure false alarms, test different drivers and lighting conditions, protect camera data and clearly state the boundary between a prototype and a production-ready product.

---

## 60-second interview answer

“Driver fatigue is dangerous because the driver may not notice that attention is reducing. Our team built a non-invasive prototype that works like a digital co-driver. A webcam observes the face, Face Mesh maps facial landmarks, and the system examines head position using pitch, yaw and roll. A Raspberry Pi processes the condition and activates a speaker when drowsiness is detected. The report states 97.5% accuracy in the straight-face position and an approximate three-second response time. My personal contribution was [ADD YOUR TRUE CONTRIBUTION]. The project taught me not only computer vision and embedded-system design, but also the importance of honest evaluation, false-alarm testing, privacy and safety limitations.”

---

## STAR answer for a technical challenge

Use this only after adding a real challenge you personally experienced.

### Situation

During testing, `[DESCRIBE THE REAL PROBLEM]`.

### Task

I needed to determine whether the issue came from the camera, facial-landmark detection, head-pose thresholds, Raspberry Pi processing or the alert hardware.

### Action

I:
- reproduced the problem consistently;
- checked each stage separately;
- reviewed the camera feed and facial landmarks;
- compared head angles with the configured threshold;
- tested the speaker independently;
- changed one variable at a time;
- recorded the result after every change.

### Result

`[DESCRIBE THE VERIFIED RESULT]`.

### Learning

This taught me to isolate a complex system into smaller modules instead of changing everything at once.
