# Dataset Information

## Overview

This dataset was created for training an object detection model in a kitchen environment.

---

## Dataset Size

* Total images: ~300–400
* Classes: 3–5
* Annotation format: YOLO

---

## Data Collection

Images were collected manually using:

* Mobile phone camera
* Indoor kitchen environment

---

## Variations Covered

The dataset includes:

* Different lighting conditions
* Various object orientations
* Multiple distances (near/far)
* Background clutter
* Partial occlusions

---

## Challenges

* Some images are visually similar (limited diversity)
* Lighting conditions not fully balanced
* Certain classes have fewer examples

---

## Preprocessing

* Duplicate removal (perceptual hashing)
* Manual filtering of low-quality images
* Data augmentation during training

---

## Data Augmentation

Applied during training:

* Horizontal flip
* Scaling
* Color jitter (HSV)
* Translation

---

## Notes

The dataset is continuously evolving and not considered complete.
Future improvements will focus on diversity rather than size.

