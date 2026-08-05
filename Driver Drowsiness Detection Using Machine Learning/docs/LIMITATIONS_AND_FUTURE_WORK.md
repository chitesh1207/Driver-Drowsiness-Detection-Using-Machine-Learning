# Limitations and Future Work

## Current limitations

- The reported 97.5% accuracy is limited to the straight-face position.
- The supplied report does not provide a full confusion matrix, precision, recall or F1-score.
- The exact sample size and participant diversity for the prototype result are not clearly documented in the supplied report.
- Camera systems may be affected by low light, glare, camera placement and motion blur.
- Facial landmarks may be less reliable with glasses, sunglasses, masks or partial occlusion.
- Head movement alone can create false alarms when a driver checks mirrors, controls or the dashboard.
- A fixed threshold may not suit every driver's natural behaviour.
- A prototype alarm does not guarantee that a driver will respond safely.
- The system is not certified for safety-critical deployment.

## Recommended future evaluation

- Test with an independent train/validation/test design.
- Prevent the same person's frames from appearing in both training and testing.
- Report confusion matrix, precision, recall, specificity, F1-score and ROC-AUC.
- Measure false alarms per hour.
- Test day, night, glare and low-light conditions.
- Include different ages, skin tones, face shapes and eyewear.
- Compare performance with and without personalised calibration.
- Measure processing speed on the Raspberry Pi.
- Validate alarm latency from detection to sound.
- Conduct all testing in a simulator or stationary vehicle, not on public roads.

## Product improvements

- Fuse Eye Aspect Ratio, Mouth Aspect Ratio and head pose.
- Add infrared or low-light camera support.
- Add driver-specific baseline calibration.
- Add confidence scoring and multi-stage alarms.
- Log only necessary events rather than storing full video.
- Add a fleet dashboard with privacy-preserving summaries.
- Add an emergency escalation workflow only after safety and legal review.
