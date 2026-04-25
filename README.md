# 🍽️ Indian Food Image Recognition using MobileNetV2

This project implements a deep learning-based approach for **Indian food classification** using **MobileNetV2**. It explores how **regional specialization (North vs South Indian cuisine)** impacts model performance.

---

## 📌 Overview

Indian cuisine is highly diverse and visually complex, making classification a challenging fine-grained task. This project evaluates performance across:

- Full dataset (89 classes)
- North Indian subset (66 classes)
- South Indian subset (21 classes)

---

## 🚀 Key Features

- MobileNetV2 with transfer learning
- Progressive fine-tuning strategy
- Comparative regional analysis
- Evaluation using Accuracy and F1-score
- Training and validation performance visualization

---

## 🗂️ Repository Structure

- `full_dataset_model.ipynb` → Full dataset training
- `north_indian_model.ipynb` → North Indian model
- `south_indian_model.ipynb` → South Indian model
- `figures/` → Plots and diagrams
- `README.md`

---

## 🧠 Model Details

- Architecture: MobileNetV2 (ImageNet pre-trained)
- Input size: 224 × 224
- Batch size: 32
- Optimizer: Adam
- Loss: Cross-Entropy Loss

### Training Strategy:
1. Freeze backbone → train classifier  
2. Unfreeze all layers → fine-tune  
3. Apply learning rate scheduling  

---

## 📊 Results Summary

| Dataset        | Classes | Accuracy | F1 Score |
|---------------|--------|----------|----------|
| Full Dataset  | 89     | 81.11%   | 79.82%   |
| North Indian  | 66     | 81.91%   | 80.89%   |
| South Indian  | 21     | **84.68%** | **84.44%** |

**Insight:** Regional specialization improves classification performance.

---

## 📂 Dataset

Multi-source Indian food dataset collected from public platforms (Kaggle, Hugging Face, etc.) and refined to 89 classes. 
Email for Dataset.

---

## ▶️ How to Run

Clone the repository:

    git clone https://github.com/your-username/indian-food-classification.git
    cd indian-food-classification

Open Jupyter Notebook:

    jupyter notebook

Run any of the following:
- full_dataset_model.ipynb
- north_indian_model.ipynb
- south_indian_model.ipynb

---

## 🧪 Requirements

- torch
- torchvision
- numpy
- matplotlib
- scikit-learn

---

## 📌 Future Work

- Multi-modal learning (image + text)
- Hierarchical classification
- Advanced augmentation (mixup, label smoothing)
- Deployment on mobile/web

---

## ⭐ Support

If you found this useful, consider giving a ⭐ to the repository!
