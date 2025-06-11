# 🧠 Skin Disease Classification using Deep Learning  
A Capstone Project | AI Summer School 2025

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow)
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)

---

## 📌 Project Overview

This project focuses on **classifying skin diseases** using dermoscopic images from the **HAM10000 dataset**. We implemented a **Convolutional Neural Network (CNN)** to identify 7 types of skin lesions, supporting the healthcare domain with automated diagnosis aid.

---

## 🧪 Problem Statement

> Can we build a deep learning model that accurately classifies dermoscopic images of skin lesions into various disease categories using a CNN architecture?

---

## 🎯 Motivation

- Early detection of skin diseases like melanoma can **save lives**.
- **Dermoscopic image analysis** is time-consuming and requires expert knowledge.
- AI-powered models can assist dermatologists for **faster and reliable** diagnosis.

---

## 🧬 Dataset: HAM10000

- **Source**: Harvard Dataverse ([Link](https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000))
- **Total Images**: 10,015 dermoscopic images
- **Classes**:
  - Actinic keratoses
  - Basal cell carcinoma
  - Benign keratosis-like lesions
  - Dermatofibroma
  - Melanocytic nevi
  - Melanoma
  - Vascular lesions

---

## 🏗️ Model Architecture

Input Layer → Conv2D → MaxPooling → Dropout
→ Conv2D → MaxPooling → Flatten
→ Dense Layer → Output Softmax Layer (7 classes)
Image Size: 64×64 RGB

Framework: TensorFlow + Keras

Loss Function: Categorical Cross-Entropy
Optimizer: Adam
Activation: ReLU, Softmax

✅ Accuracy Graph

Training Accuracy: ~67.5%
Validation Accuracy: ~68.2%
Performance is consistent with room for improvement via hyperparameter tuning or transfer learning.

![image](https://github.com/user-attachments/assets/ce8f5d1a-ea29-4b9e-a884-1eead55764c8)

🧪 Sample Predictions

| Image | Actual   | Predicted | Confidence |
| ----- | -------- | --------- | ---------- |
| 🖼️   | Melanoma | Melanoma  | 91.2%      |
| 🖼️   | Nevi     | Nevi      | 87.5%      |


