# 🧠 Eye Disease Classification using DeiT Tiny

This project uses a Vision Transformer (DeiT Tiny) to classify fundus images into four eye disease categories: **Cataract**, **Glaucoma**, **Diabetic Retinopathy**, and **Normal**.

---

## 📁 Dataset Structure

Dataset should follow this format:

dataset/
├── cataract/
├── diabetic_retinopathy/
├── glaucoma/
└── normal/

---

## 🔧 Key Features

- **Model**: DeiT Tiny (`deit_tiny_patch16_224`) pretrained on ImageNet
- **Transformations**: Random horizontal flip, rotation, resized crop, normalization
- **Loss**: CrossEntropy with Label Smoothing (0.05)
- **Optimizer**: Adam with weight decay and ReduceLROnPlateau scheduler
- **Training Enhancements**: Early stopping and best model checkpointing
- **Evaluation**:
  - Accuracy
  - Confusion Matrix
  - Classification Report
  - ROC-AUC (per class and macro-average)

---

## 📊 Example Results

Final Training Accuracy: 97.85%
Final Validation Accuracy: 95.62%
Test Accuracy: 95.58%
Test AUC Score: 0.9959
