# UCB Traffic Sign Recognition

A computer vision project that classifies traffic sign images, developed as part of the
Post Graduate Certificate in Machine Learning and AI at UC Berkeley Executive Education
(via Emeritus).

## Problem Statement

Self-driving cars and driver-assistance systems (ADAS) need to automatically recognize
traffic signs from camera images to make correct driving decisions — for example,
adjusting speed at a speed limit sign. This project builds a step toward that capability.

## Current Stage: Binary Classification

As a first milestone before tackling full multi-class recognition, this stage classifies
images into two categories:
- **Speed Limit Sign** (any of the 9 speed limit sign types in the dataset)
- **Other Sign** (all remaining sign types)

This simpler framing validates the end-to-end pipeline — data loading, preprocessing,
model training, and evaluation — before scaling up to full 43-class recognition.

## Dataset

**German Traffic Sign Recognition Benchmark (GTSRB)**, via
[Kaggle](https://www.kaggle.com/datasets/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign) —
~50,000 images across 43 sign classes, regrouped here into 2 categories.

## Approach

- EDA on class distribution and image metadata
- Binary CNN classifier (speed limit vs. other)
- Evaluation via confusion matrix and classification report

## Results

The model achieved **99.41% accuracy** on the held-out test set — meaning it correctly
classified nearly all traffic sign images into "Speed Limit" vs. "Other," including
images it had never seen during training
