
# Vehicle Smoke Detection using DB-Net

## Overview

This project implements a deep learning–based vehicle smoke detection system for identifying smoke-emitting vehicles from road surveillance images. Instead of relying on traditional bounding-box detection, the system performs **block-wise smoke localization**, enabling more precise identification of smoke regions in complex traffic scenes. The project is relevant to smart city monitoring, environmental regulation, and intelligent transportation systems.

---

## Key Features

* Block-wise smoke detection using grid-based labeling
* Custom preprocessing pipeline for segmentation-to-grid conversion
* DB-Net architecture with multi-scale feature aggregation
* ResNet-50 backbone for feature extraction
* Weighted loss to handle class imbalance
* IoU-based evaluation metrics
* Visual overlay of smoke predictions on images

---

## Dataset Processing

* Input images and pixel-level smoke masks are resized to a fixed resolution
* Masks are divided into grid blocks
* Each block is labeled as smoke or non-smoke based on pixel density
* Processed images and labels are stored for efficient training

---

## Model Architecture

* **Architecture:** DB-Net (Dual-Branch Network)
* **Backbone:** ResNet-50
* **Task:** Block-wise binary classification (smoke / no-smoke)
* **Framework:** PyTorch

---

## Training & Evaluation

* Custom PyTorch Dataset and DataLoader
* Data augmentation and normalization
* Adam optimizer with learning rate scheduling
* Model checkpointing and resume support
* Performance evaluation using Intersection over Union (IoU)

---

## Technologies Used

* Python
* PyTorch
* OpenCV
* NumPy
* Google Colab
* Deep Learning
* Computer Vision

---

## Applications

* Smart city traffic surveillance
* Vehicle emission monitoring
* Environmental pollution detection
* Intelligent transportation systems

---

## Future Work

* Real-time inference on video streams
* Backend deployment using FastAPI
* Integration with traffic management systems
* Edge-device optimization


Just tell me ✨
