# 👁️ Computer Vision Pipeline: Object Detection, Semantic Segmentation & Web App Integration

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1thSX6_vNXhldC-AgeMyD5ob3fK_L0XQW?usp=sharing)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-Latest-red.svg)](https://pytorch.org/)
[![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green.svg)](https://opencv.org/)

An end-to-end Deep Learning Computer Vision solution covering both **Object Detection** and **Semantic/Instance Segmentation** workflows. This project includes data preprocessing, baseline model surveys, model comparison, advanced fine-tuning with 3 optimization strategies, quantitative testing, and a web application interface for deployment.

---

## 📌 Table of Contents
- [PART 1: OBJECT DETECTION](#-part-1-object-detection)
  - [I. Setup \& Data Preprocessing](#i-setup--data-preprocessing)
  - [II. Model Survey \& Training](#ii-model-survey--training)
  - [III. Performance Comparison](#iii-performance-comparison)
  - [IV. Inference Testing on Arbitrary Video](#iv-inference-testing-on-arbitrary-video)
- [PART 2: SEGMENTATION](#-part-2-segmentation)
  - [I. Mask Setup \& Preprocessing](#i-mask-setup--preprocessing)
  - [II. Model Survey](#ii-model-survey)
  - [III. Post-Survey Metrics Comparison](#iii-post-survey-metrics-comparison)
  - [IV. Advanced Fine-Tuning (3 Strategies)](#iv-advanced-fine-tuning-3-strategies)
  - [V. Quantitative Testing](#v-quantitative-testing)
- [PART 3: WEB APPLICATION INTERFACE](#-part-3-web-application-interface)
- [🚀 How to Run](#-how-to-run)

---

## 🎯 PART 1: OBJECT DETECTION

### I. Setup & Data Preprocessing
- **Data Pipeline:** Loading image datasets, bounding box annotation parsing, and data cleaning.
- **Preprocessing & Augmentation:** Image resizing, normalization, bounding box scaling, and data augmentation.
- **Data Visualization:** Overlaying bounding boxes and class labels onto raw images for dataset verification.

### II. Model Survey & Training
- Surveying candidate object detection architectures (e.g., YOLO variants, Faster R-CNN, SSD).
- Setting up loss functions (bounding box regression loss + classification loss) and training pipelines.

### III. Performance Comparison
- Benchmarking models across standard detection metrics: **mAP@50**, **mAP@50-95**, **Precision**, **Recall**, and **FPS**.

### IV. Inference Testing on Arbitrary Video
- Running frame-by-frame object detection on custom input videos.
- Rendering dynamic bounding boxes, confidence scores, and exporting annotated output videos.

---

## ✂️ PART 2: SEGMENTATION

### I. Mask Setup & Preprocessing
- **Mask Generation & Parsing:** Converting annotations into binary/multi-class segmentation masks.
- **Preprocessing:** Normalization, mask alignment, and data augmentation tailored for pixel-level prediction.
- **Visualization:** Overlaying ground truth segmentation masks onto input images.

### II. Model Survey
- Surveying semantic/instance segmentation architectures (e.g., U-Net, Mask R-CNN, DeepLabV3+).
- Loss function setup (e.g., Dice Loss, Cross-Entropy Loss, Focal Loss).

### III. Post-Survey Metrics Comparison
- Comparing baseline segmentation models across key evaluation metrics: **IoU (Intersection over Union)**, **mIoU**, **Dice Coefficient / F1-Score**, and **Pixel Accuracy**.

### IV. Advanced Fine-Tuning (3 Strategies)
Implementing 3 advanced fine-tuning strategies to boost model performance:
1. **Data Augmentation Strategy:** Applying geometric and photometric transformations to prevent overfitting.
2. **Layer Unfreezing / Backbone Adaptation:** Selectively or fully unfreezing pre-trained backbone features.
3. **Optimized Learning Rate Scheduling:** Utilizing small learning rates with warmups or cosine annealing to fine-tune weights smoothly without destructive updates.

### V. Quantitative Testing
- Rigorous quantitative evaluation on unseen test datasets.
- Qualitative inspection of predicted segmentation masks vs. ground truth.

---

## 🌐 PART 3: WEB APPLICATION INTERFACE

- Building an interactive web display interface (e.g., Streamlit / Gradio / Flask) to showcase real-time prediction capabilities.
- Supports image upload, video stream processing, and interactive visual rendering of Object Detection bounding boxes and Segmentation overlays.

---

## 🚀 How to Run

Click the badge below to open and execute the complete interactive notebook directly in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1thSX6_vNXhldC-AgeMyD5ob3fK_L0XQW?usp=sharing)
