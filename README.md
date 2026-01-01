# 🏥 IoT-Based Healthcare Kit for Cardiac Diagnosis
> **Published in IEEE Xplore** | Developed at PES University | Licensed to Texas A&M University

[![IEEE Xplore](https://img.shields.io/badge/Publication-IEEE%20Xplore-maroon.svg)](https://ieeexplore.ieee.org/)
[![Tech Stack](https://img.shields.io/badge/Stack-IoT%20%7C%20ML%20%7C%20Embedded-blue.svg)](#)
[![Accuracy](https://img.shields.io/badge/Best%20Accuracy-78.67%25-orange.svg)](#)

## 🔍 Project Overview
Cardiovascular diseases (CVD) and Cardiac Arrhythmia are leading causes of mortality worldwide. This project implements a hardware-software integrated system for **24/7 cardiac monitoring**. By utilizing ECG sensors and machine learning, the system provides early diagnosis, allowing for preventative lifestyle changes and medical intervention.

## 🏗 System Architecture & Stack
The project bridges the gap between medical signal acquisition and automated data analysis:

* **Hardware Layer:** ECG Sensors (signal acquisition), Arduino (data processing), Raspberry Pi (computational hub).
* **Signal Processing:** Real-time peak detection in ECG waveforms to extract vital cardiac attributes.
* **ML Framework:** Python-based models trained on the **UCI Machine Learning Repository**.
* **Dimensionality Reduction:** Principal Component Analysis (PCA) for optimized feature extraction in Arrhythmia classification.

## 🤖 Machine Learning Performance
We evaluated several algorithms to determine the most reliable model for clinical decision support.

### 1. Cardiovascular Disease (CVD) Prediction
*Binary Classification: (0: Healthy, 1: At Risk)*

| Rank | Model | Accuracy |
| :--- | :--- | :--- |
| **01** | **Linear Support Vector Machine (SVM)** | **78.67%** |
| 02 | Random Forest Classifier | 77.33% |
| 03 | Logistic Regression | 76.00% |
| 04 | K-Nearest Neighbors (KNN) | 74.67% |
| 05 | Decision Tree | 70.67% |

### 2. Cardiac Arrhythmia Prediction
*Multi-class Classification: 16 distinct cardiac categories.*

| Algorithm | Configuration | Accuracy |
| :--- | :--- | :--- |
| **Linear SVM** | **Regularization (C=0.01)** | **74.00%** |
| Random Forest | Combined with SVM | 73.00% |
| Polynomial SVM | Degree Kernel | 68.00% |
| RBF SVM | Radial Basis Function | 66.00% |

## 📈 Key Conclusions
* **Optimal Algorithm:** The **Support Vector Machine (SVM)** consistently outperformed other models, proving most effective at handling the high-dimensional attributes of ECG data.
* **Rural Impact:** The framework is designed for high-efficiency monitoring in rural areas where access to specialized cardiologists is limited.
* **Internet of Things:** Integration with IoT improves administrative efficiency and operational patient care.

## 🔮 Future Enhancements
* Implementation of **Deep Learning (CNN/LSTM)** for automated ECG pattern recognition.
* Data augmentation to expand the training set for rarer arrhythmia classes.
* Development of a mobile-first dashboard for real-time patient-doctor alerts.

---

### 🎓 Academic Citation
Authorized licensed use limited to: **Texas A&M University**. 
*Originally presented at the 2022 IEEE 4th Eurasia Conference on Biomedical Engineering, Healthcare and Sustainability (ECBIOS).*
