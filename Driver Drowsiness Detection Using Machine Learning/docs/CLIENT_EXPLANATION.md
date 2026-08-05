# Explaining the Project to a Non-Technical Client

## One-sentence explanation

This is like a digital co-driver: a camera watches for visible signs that the driver is becoming sleepy, and a small computer sounds an alarm before the driver completely loses attention.

## Real-world example

Imagine a delivery driver working a long night shift. The driver begins to nod forward slowly but may not realise it. A dashboard camera captures the face. The system checks facial landmarks and head position. When the head remains in a drowsy position long enough to cross the configured threshold, the Raspberry Pi activates a speaker. The warning tells the driver to stop safely and rest.

## Explain every component simply

| Technical component | Client-friendly explanation |
|---|---|
| Webcam | The system's eyes |
| Face Mesh | A digital map that places reference points on the face |
| Facial landmarks | Measuring points around the eyes, nose, mouth and face |
| Head pose | The direction in which the driver's head is pointing |
| Pitch | Looking up or down |
| Yaw | Looking left or right |
| Roll | Tilting the head toward a shoulder |
| Threshold | The safety limit that decides when normal movement becomes concerning |
| Raspberry Pi | A small computer that performs the checks |
| Speaker | The warning device |
| Machine learning | A method for recognising patterns linked to alert and drowsy behaviour |

## Three-minute client presentation

“Fatigue develops gradually. A driver may blink slowly, yawn or begin nodding before falling asleep. The challenge is that the driver may not notice these warning signs.

Our prototype acts like a digital co-driver. A camera observes the driver's face without attaching sensors to the body. Face Mesh creates a map of facial landmarks. The system then checks the head direction and visible drowsiness patterns. A Raspberry Pi processes the information, and when the configured warning condition is met, a speaker sounds an alarm.

The project report recorded 97.5% accuracy for a straight-face position and an approximate response time of three seconds. I would explain that honestly as a prototype result under limited conditions. It still needs stronger testing under poor lighting, different head angles, glasses and a larger range of drivers before it could be considered for real-world safety use.

The main value of the project is that it demonstrates a low-cost, non-invasive way to provide an early warning. The next development step would be broader testing, fewer false alarms, stronger privacy controls and integration with fleet-safety reporting.” 

## Business value

- Gives an early warning when fatigue signs appear
- Does not require electrodes or wearable sensors
- Can be built from relatively low-cost hardware
- Could support individual drivers, transport operators and fleet-safety teams
- Can provide event data for safety training and risk analysis

## Questions a client may ask

### “Does it guarantee that accidents will not happen?”

No. It is an assistance system, not a guarantee. Drivers must still stop safely and rest.

### “Does it record the driver's face?”

The prototype uses live camera input. A production design should minimise storage, process data locally where possible and clearly define retention and consent.

### “Will it work at night?”

Low light is a known challenge for image-based systems. Night-time use would require suitable cameras and controlled testing.

### “What happens when a driver simply looks down?”

The system should use duration and repeated patterns rather than one movement. Better versions should combine head pose with eyes and yawning to reduce false alarms.

### “Why use a camera instead of body sensors?”

A camera is non-invasive: the driver does not need to wear electrodes or special equipment.

### “What did you personally do?”

Give only a truthful answer based on your contribution. Use:
“I worked on [YOUR MODULE], completed [YOUR TESTING], and helped produce [YOUR DOCUMENTATION/DIAGRAM].”
