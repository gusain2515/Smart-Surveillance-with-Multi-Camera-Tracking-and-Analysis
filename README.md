# Multi-Stream Camera System with Object Detection and Tracking
This project implements a multi-stream camera system capable of real-time object detection, tracking, and demographic analysis using computer vision and deep learning. It processes multiple RTSP streams to detect individuals, track their movements, and predict their gender and age. The system is designed for applications such as retail analytics, surveillance, and crowd management.
# Features
Multi-Camera Stream Handling: Supports multiple RTSP streams for concurrent video processing.

Real-Time Object Detection and Tracking: Utilizes the YOLO model with ByteTrack for accurate person detection and tracking.

Demographics Analysis:
Gender classification using a custom-trained YOLO model on full-body images.

Age estimation using the DeepFace library.

# Data Logging:
Saves tracking and demographic data to CSV files.

Rotates and archives data at regular intervals.

# Visualization:
Displays video streams with detection boxes, grid overlays, and demographic annotations.

Failsafe Mechanism: Automatically detects and handles camera disconnections.

# Custom Gender Prediction Model
# Model Overview
The gender prediction model used in this project is a custom-trained YOLO model designed to classify male and female genders. Unlike conventional gender classification models that rely on facial features, this model is trained on a dataset containing whole-body images of individuals. This approach provides the following benefits:

Adaptability: Works in scenarios where the face is obscured or not visible.
Diverse Use Cases: Suitable for wide-angle cameras capturing individuals in varied postures and lighting conditions.
Training Dataset
The training dataset for this model includes:

Class Labels: Male and Female.
Data Sources: Curated from publicly available datasets and proprietary sources, ensuring diverse poses, clothing, and backgrounds.
Annotations: Bounding boxes and labels for the whole body

And uses Optuna framework for hyperparameter tuning
