# Failure Case Analysis

## Overview

This document analyzes typical failure cases observed during model inference.

Understanding these limitations is essential for improving robustness in real-world robotic systems.

---

## 1. Low-Light Conditions

### Issue

Detection performance drops significantly in poor lighting.

### Reason

Training data lacks sufficient low-light examples.

---

## 2. Partial Occlusion

### Issue

Objects are missed when partially covered.

### Example

* Object behind another item
* Only part of object visible

---

## 3. Small Objects / Far Distance

### Issue

Objects far from the camera are often missed.

### Reason

Limited representation of small-scale objects in training data.

---

## 4. Visual Similarity Confusion

### Issue

Model confuses objects with similar shapes or colors.

### Example

* Similar kitchen items

---

## 5. Background Clutter

### Issue

Busy backgrounds reduce detection accuracy.

---

## Key Insight

Most errors are caused by:

> Lack of dataset diversity rather than model capacity.

---

## Future Improvements

* Add more diverse training samples
* Include edge cases intentionally
* Balance class distribution
* Improve annotation quality
