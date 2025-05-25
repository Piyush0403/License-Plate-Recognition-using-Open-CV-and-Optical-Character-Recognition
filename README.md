# License-Plate-Recognition-using-Open-CV-and-Optical-Character-Recognition
A real-time Computer Vision system designed to automate the detection of unregistered vehicles in ASU Lot 59. By combining YOLOv8 (for plate detection) and PaddleOCR (for character recognition), this project reduces manual enforcement workload and improves detection speed and accuracy.

# Overview
- ASU’s Lot 59 handles over 6,000 vehicles daily, making manual license plate checks inefficient, error-prone, and unsustainable. Our solution introduces a camera-cart-based system that:
  - Detects license plates in real time using YOLOv8
  - Reads text from plates using PaddleOCR
  - Compares against a list of registered vehicles
  - Flags unregistered cars instantly for staff intervention

# Tech Stack
- YOLOv8 – License plate detection
- PaddleOCR – Optical character recognition
- OpenCV – Preprocessing and image pipeline
- Python (Jupyter Notebooks) – Implementation and testing

# Success Metrics

| Metric                         | Target Value |
| ------------------------------ | ------------ |
| Detection Accuracy             | ≥ 95%        |
| OCR Accuracy                   | ≥ 92%        |
| Matching Accuracy              | ≥ 90%        |
| Manual Patrol Time Reduction   | ≥ 70%        |
| Staff Efficiency Improvement   | ≥ 50%        |
| Alert Latency (Capture → Flag) | ≤ 5 seconds  |

# Methodology
- Plate Detection
  - YOLOv8 identifies and crops license plates from cart-mounted camera video feeds.
- Text Extraction
  - PaddleOCR reads alphanumeric content from detected plates.
-Database Matching
  - Extracted text is matched against a list of registered vehicle plates (CSV format).
-Classification & Logging
  - Vehicles are marked as Registered or Unregistered, and logs are generated in real time.

# Hardware Setup
- Cart-mounted HD cameras (e.g., Axis P1445-LE-3, Hikvision)
- Laptop/Mini-PC for model inference
- Solar panels + battery inverter for sustained power
- Optional: Real-time cloud integration

# Key Features
- Fully automated workflow: from capture to classification
- Works in varying lighting and weather conditions
- Scalable to other ASU parking zones or campuses
- Built-in alerting system for enforcement teams


# Files in This Repo
- CIS515-Team4-Final.ipynb – Final code notebook (YOLOv8 + PaddleOCR)
- Team005FinalProjectDeck.pdf – Slide deck presentation
- README.md – Project documentation

# Future Scope
- Autonomous cart navigation
- Expand coverage across all ASU parking lots
- Real-time cloud syncing and analytics dashboard
- Integration with ASU permit management system


