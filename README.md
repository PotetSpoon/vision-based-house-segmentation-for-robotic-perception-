# Real-Time Object Detection for Robotic Perception

## Overview

This project implements a YOLO-based object detection system designed for real-time robotic perception in a kitchen environment.

The goal is to simulate a vision module that could be integrated into assistive robotics systems, such as exoskeletons or humanoid robots, enabling interaction with everyday objects.

---

## Demo

### 🎥 Real-Time Detection

(Add your demo video or GIF here)

* Webcam-based real-time detection
* Bounding boxes + confidence scores
* Instance segmentation (if enabled)

---

## Features

* Real-time object detection using YOLO
* Custom dataset (kitchen environment)
* Designed for robotic perception pipelines
* Supports multiple object classes
* Modular inference pipeline

---

## Project Structure

```
project/
│
├── README.md
├── requirements.txt
│
├── models/
│   └── best.pt
│
├── data/
│   └── dataset_info.md
│
├── src/
│   ├── train.py
│   ├── inference.py
│   ├── utils.py
│
├── demo/
│   ├── demo_video.mp4
│   └── images/
│
├── results/
│   ├── metrics.png
│   ├── confusion_matrix.png
│   └── predictions/
│
└── analysis/
    └── failure_cases.md
```

---

## Model Performance

| Metric    | Value     |
| --------- | --------- |
| mAP@50    | 0.56–0.58 |
| Precision | 0.60–0.66 |
| Recall    | 0.52–0.53 |

> Note: Performance varies depending on dataset version and data quality.

---

## Dataset

* Custom collected dataset (~300–400 images)
* Kitchen environment
* Annotated manually

Focus on variability:

* Lighting conditions
* Object distance
* Occlusion
* Background clutter

More details in: `data/dataset_info.md`

---

## Installation

```bash
git clone <your-repo>
cd project

pip install -r requirements.txt
```

---

## Usage

### Run inference (webcam)

```bash
python src/inference.py --source webcam
```

### Run inference (image)

```bash
python src/inference.py --source path/to/image.jpg
```

---

## Design Considerations

This project is structured as a simplified perception module for robotics:

* Input: camera stream
* Processing: object detection model
* Output: structured detections (bounding boxes, classes)

This modularity allows integration with:

* control systems
* planning modules
* human-robot interaction systems

---

## Limitations

* Reduced performance in low-light conditions
* Difficulty with partially occluded objects
* Confusion between visually similar classes
* Limited dataset size

See detailed analysis: `analysis/failure_cases.md`

---

## Future Work

* Improve dataset diversity
* Add temporal tracking (video-based)
* Integrate with ROS pipeline
* Optimize for edge devices
* Expand to more object classes

---

## Motivation

This project is part of a broader goal:

> Building perception systems for assistive robotics, including exoskeletons and humanoid robots.

---

## License

MIT License (or your choice)
