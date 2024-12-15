Objective:
Develop a computer vision system to monitor safety compliance on construction sites by detecting safety vests and helmets, and saving videos of detected violations for review.

Description:
The project employs YOLOv5, trained on a dataset from Roboflow, to detect safety gear on construction workers in real-time. It not only generates alerts for violations but also records and stores video clips of these incidents for documentation and future analysis.

Dataset Preparation:

Used Roboflow to annotate and preprocess a dataset of workers with and without safety vests and helmets.
Included diverse environmental and lighting conditions for robustness.
Model Training and Deployment:

Trained YOLOv5 on the annotated dataset using transfer learning for high-accuracy detection.
Integrated the trained model with a real-time video feed via OpenCV.
Violation Detection and Recording:

Continuously monitors the video feed to detect workers missing helmets or vests.
Records short video clips (e.g., 10-15 seconds) of each detected violation, tagged with timestamps for easy retrieval.
Alerts and Reporting:

Sends real-time alerts (e.g., notifications or sound alarms) upon detecting violations.
Stores videos in a structured format for managers to review incidents and analyze patterns.
Technology Stack:

Dataset Handling: Roboflow for annotation and augmentation.
Model: YOLOv5 for object detection.
Video Processing: OpenCV for real-time detection and recording.
Backend: Python for integration and video storage management.
Impact:

Ensures construction site safety by monitoring compliance with minimal manual intervention.
Provides evidence of safety violations for auditing and corrective actions.
Improves accountability and promotes a culture of safety.
