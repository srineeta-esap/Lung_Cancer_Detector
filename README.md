# 🩺 Lung Cancer Detector using CNN

This project uses a **Convolutional Neural Network (CNN)** to detect and classify lung tissue images into three categories:

- **Normal**
- **Lung Adenocarcinoma (lung_aca)**
- **Lung Squamous Cell Carcinoma (lung_scc)**

---

## 🧠 Project Overview

Histopathological images were used to train a deep learning model to classify lung cancer types. The model is built with **TensorFlow/Keras**, and includes visualization, preprocessing, training, evaluation, and reporting.

---

## 📁 Dataset

- **Classes**:
  - `lung_n`: Normal tissue
  - `lung_aca`: Adenocarcinoma
  - `lung_scc`: Squamous cell carcinoma

---

## 🛠 Tech Stack

- Python
- TensorFlow & Keras
- OpenCV
- NumPy, Pandas, Matplotlib
- scikit-learn

---

## 📊 Model Architecture

- 3 × `Conv2D` + `MaxPooling2D` layers
- `Flatten` + `Dense` layers
- `BatchNormalization` & `Dropout` to prevent overfitting
- `Softmax` activation for multiclass classification

---

## 🔍 Features

- Early stopping if validation accuracy > 90%
- ReduceLROnPlateau to dynamically reduce learning rate
- Classification report with precision, recall, F1-score

---

## 📈 Results

- **Training Accuracy**: Approached ~100%
- **Validation Accuracy**: Stabilized around **90%**
- High precision on normal class; slight imbalance in cancer class recall.
