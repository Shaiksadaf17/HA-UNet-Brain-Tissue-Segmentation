# 🧠 HA-UNet: Hybrid-Attention U-Net for Few-Shot 3D Brain Tissue Segmentation

A lightweight deep learning architecture for **3D Brain MRI Segmentation** that combines **Depthwise-Separable Convolutions**, a **Transformer Bottleneck**, and **CBAM Attention** to improve segmentation accuracy while reducing GPU memory usage.

---

## 📌 Project Overview

Brain tissue segmentation is an important task in medical imaging that helps identify different brain structures from MRI scans. Accurate segmentation can assist doctors and researchers in disease diagnosis, treatment planning, and brain image analysis.

In this project, I developed **HA-UNet**, a hybrid CNN-Transformer architecture designed for the **MRBrainS13** dataset under a **few-shot learning** setting, where only a small number of labelled MRI scans are available.

The proposed architecture combines:

- Residual Depthwise-Separable 3D Convolutions
- Lightweight Transformer Bottleneck
- CBAM Attention Modules
- Dice + Focal + Cross Entropy Loss
- Foreground-balanced Patch Sampling
- Gaussian Sliding Window Inference

---

## 🚀 Features

- Hybrid CNN–Transformer Architecture
- Memory-Efficient 3D U-Net
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

**Dataset:** MRBrainS13

### MRI Modalities

- T1
- T1-IR
- T2-FLAIR

### Brain Tissue Classes

- White Matter
- Cortical Grey Matter
- Cerebrospinal Fluid (CSF)
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
| Loss Function | Dice + Focal + Cross Entropy |
| Patch Size | 64 × 64 × 64 |
| Batch Size | 2 |
| Epochs | 150 |
| Validation | Leave-One-Out Cross Validation (LOOCV) |

---

## ▶️ How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/HA-UNet-Brain-Tissue-Segmentation.git
cd HA-UNet-Brain-Tissue-Segmentation
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Open Google Colab

Upload or open:

```
notebooks/HA_UNet_Training.ipynb
```

### 4. Prepare the Dataset

Download the **MRBrainS13** dataset and place it in the required directory.

> **Note:** Update the dataset paths inside the notebook if necessary.

### 5. Run the Notebook

Run all cells from top to bottom.

The notebook performs:

- Data preprocessing
- Data augmentation
- Model training
- Leave-One-Out Cross Validation (LOOCV)
- Model evaluation
- Performance visualization

---

## 📊 Results

| Metric | Value |
|---------|-------|
| Mean Dice Score | **0.847** |
| HD95 | **4.21 mm** |
| GPU Memory | **8.1 GB** |
| Dice Improvement over 3D U-Net | **+4.3%** |
| GPU Memory Reduction | **28%** |

---

## 📈 Outputs

After training, the notebook generates:

- Training & Validation Loss Curves
- Validation Dice Curves
- Dice Score Evaluation
- HD95 Evaluation
- Model Performance Graphs
- Training Logs

---

## 🛠️ Technologies Used

- Python
- PyTorch
- MONAI
- NumPy
- Matplotlib
- SimpleITK
- Deep Learning
- Computer Vision
- Medical Image Processing

---




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

📧 Email: shaiksadafpatel786@gmail.com



---

## ⭐ Support

If you found this project helpful or interesting, please consider giving this repository a ⭐.
