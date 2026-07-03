# 🧠 HA-UNet: Hybrid-Attention U-Net for Few-Shot 3D Brain Tissue Segmentation

A lightweight hybrid deep learning architecture for **3D brain MRI segmentation** that combines **Depthwise-Separable Convolutions**, **Transformer Bottleneck**, and **CBAM Attention** to improve segmentation accuracy while reducing GPU memory usage.

---

## 📌 Project Overview

Brain tissue segmentation plays a crucial role in medical image analysis, disease diagnosis, and surgical planning.

This project proposes **HA-UNet**, a hybrid CNN-Transformer architecture designed for the **MRBrainS13 dataset** under an extreme few-shot learning setting.

The model combines:

- Residual Depthwise-Separable 3D Convolutions
- Lightweight Transformer Bottleneck
- CBAM Attention
- Dice + Focal + Cross Entropy Loss
- Foreground-balanced Patch Sampling
- Gaussian Sliding Window Inference

---

## 🚀 Features

- Memory Efficient Hybrid U-Net
- Transformer-based Global Context Learning
- CBAM Attention Mechanism
- Multi-modal MRI Segmentation
- Few-shot Learning
- 3D Medical Image Segmentation
- PyTorch + MONAI Implementation

---

## 🏗️ Model Architecture

```
Input MRI
      │
      ▼
Depthwise-Separable Encoder
      │
      ▼
Transformer Bottleneck
      │
      ▼
CBAM Attention Decoder
      │
      ▼
Segmentation Output
```

---

## 📂 Dataset

**MRBrainS13**

MRI Modalities

- T1
- T1-IR
- T2-FLAIR

Segmentation Classes

- White Matter
- Cortical Grey Matter
- CSF
- Ventricles
- Brain Stem
- Basal Ganglia
- Cerebellum
- White Matter Lesions

---

## ⚙️ Training Configuration

| Parameter | Value |
|------------|--------|
| Framework | PyTorch |
| Library | MONAI |
| Optimizer | AdamW |
| Loss | Dice + Focal + Cross Entropy |
| Patch Size | 64×64×64 |
| Batch Size | 2 |
| Epochs | 150 |
| Validation | Leave-One-Out Cross Validation |

---

## 📊 Results

| Metric | Value |
|---------|-------|
| Mean Dice Score | **0.847** |
| HD95 | **4.21 mm** |
| GPU Memory | **8.1 GB** |
| Dice Improvement | **+4.3%** |
| Memory Reduction | **28%** |

---

## 🛠️ Technologies Used

- Python
- PyTorch
- MONAI
- NumPy
- Matplotlib
- SimpleITK
- Medical Image Processing
- Deep Learning
- Computer Vision

---

## 📁 Repository Structure

```
HA-UNet-Brain-Tissue-Segmentation/
│
├── notebooks/
├── report/
├── logs/
├── images/
├── results/
├── README.md
├── requirements.txt
└── LICENSE
```

---

## 🎯 Future Improvements

- Semi-Supervised Learning
- Self-Supervised Pretraining
- Knowledge Distillation
- Clinical Validation
- Model Deployment

---

## 👨‍💻 Author

**Shaik Sadaf Patel**

MSc Artificial Intelligence

Queen Mary University of London



---

## ⭐ If you found this project useful, consider giving it a star!
