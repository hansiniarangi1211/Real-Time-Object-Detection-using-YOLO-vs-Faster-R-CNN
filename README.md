# Real-Time-Object-Detection-using-YOLO-vs-Faster-R-CNN
# Real-Time Object Detection using YOLO vs Faster R-CNN

A deep learning project that implements and compares **YOLO** and **Faster R-CNN** from scratch for real-time object detection on a custom helmet detection dataset. The project evaluates both architectures in terms of detection accuracy, inference speed, latency, and model complexity.

---

## Project Overview

The objective of this project is to build two state-of-the-art object detection models from scratch and compare their performance on a real-world safety application.

The implementation includes:

- Data preprocessing and augmentation
- Train/Validation/Test split (70/20/10)
- Custom implementation of YOLO
- Custom implementation of Faster R-CNN
- Quantitative performance evaluation
- Visual prediction analysis

---

## Dataset

**Helmet Detection Dataset**

Sources:
- https://universe.roboflow.com/ekant-swami/helmate
- https://www.kaggle.com/datasets/pkdarabi/helmet/data

Classes:
- Helmet
- No Helmet
- Person

---

## Data Preparation

The dataset preprocessing pipeline includes:

- Image preprocessing
- Bounding box annotation parsing
- Train/Validation/Test split (70/20/10)
- Data augmentation:
  - Horizontal Flip
  - Brightness Adjustment
  - Scaling
  - Random Crop

Dataset analysis includes:

- Class distribution
- Bounding box size distribution
- IoU distribution histogram

---

## YOLO Implementation

Implemented from scratch with:

- Custom CNN backbone
- Grid-based detection head
- Bounding box regression
- Objectness prediction
- Class prediction
- IoU-based localization

---

## Faster R-CNN Implementation

Implemented from scratch with:

- CNN backbone
- Anchor Generator
- Region Proposal Network (RPN)
- IoU-based anchor labeling
- ROI Pooling
- Classification head
- Bounding box regression head
- Non-Maximum Suppression (NMS)

---

## Evaluation Metrics

Both models are evaluated using:

- mAP@0.5
- Precision
- Recall
- FPS
- Inference Latency
- Model Size

Additional evaluation includes:

- Precision-Recall curves
- AP per class
- Qualitative prediction visualization
- Comparison table between YOLO and Faster R-CNN

---

## Technologies Used

- Python
- PyTorch
- NumPy
- OpenCV
- Albumentations
- Matplotlib
- Google Colab



---

## Results

The project compares the strengths and trade-offs of YOLO and Faster R-CNN in terms of:

- Detection accuracy
- Localization quality
- Inference speed
- Computational efficiency
- Overall suitability for real-time object detection

---

