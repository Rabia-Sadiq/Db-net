Vehicle Smoke Detection using DB-Net
Overview

This project implements a deep learning–based vehicle smoke detection system designed to identify smoke-emitting vehicles from road surveillance images. Unlike traditional object detection approaches, this system performs block-wise smoke localization, enabling more accurate identification of smoke regions in complex traffic environments. The solution is suitable for smart city monitoring, traffic enforcement, and environmental compliance systems.

Key Features

Block-wise smoke detection instead of bounding-box detection

Custom preprocessing pipeline for grid-based labeling

Multi-scale feature aggregation using a DB-Net architecture

Robust handling of class imbalance using weighted loss

IoU-based evaluation for performance assessment

Visualization of smoke predictions over input images

Dataset Preparation

Input images and pixel-level smoke masks are resized to a fixed resolution

Masks are divided into grid blocks

Each block is labeled as smoke or non-smoke based on smoke pixel density

Processed data is stored as resized images and NumPy grid labels

Model Architecture

Backbone: ResNet-50

Architecture: DB-Net (Dual-Branch Network)

Prediction Type: Block-wise binary classification

Loss Function: Cross-Entropy Loss with class weights

Framework: PyTorch

Training & Evaluation

Custom PyTorch Dataset and DataLoader with augmentation support

Adam optimizer with learning rate scheduling

Model checkpointing and resume support

Performance evaluated using Intersection over Union (IoU) metrics

Best-performing model saved automatically based on validation IoU

Technologies Used

Python

PyTorch

OpenCV

NumPy

Google Colab

Deep Learning

Computer Vision

Applications

Smart city traffic monitoring

Vehicle emission control systems

Environmental pollution detection

Intelligent transportation systems

Future Improvements

Real-time inference on live CCTV/video streams

Integration with traffic management systems

Deployment using FastAPI or similar backend

Edge-device optimization for faster inference
