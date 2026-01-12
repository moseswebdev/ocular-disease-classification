# 🧠 Multiclass Ocular Disease Classification Using Deep Learning & Vision Transformers

## 📌 Overview
Ocular diseases are a major cause of vision impairment worldwide, and early diagnosis is essential to prevent irreversible blindness.  
This project presents a **multiclass ocular disease classification system** using **deep learning and transformer-based architectures**, including **DenseNet201**, **ConvNeXt**, and a **custom Vision Transformer (ViT-B16)** implemented in TensorFlow/Keras.

The system classifies **10 ocular diseases** from retinal images and employs **class-weighted training, optimized fine-tuning strategies, and a weighted ensemble approach** to achieve high accuracy and strong clinical relevance.

---

## 👁️ Ocular Diseases Classified
1. Central Serous Chorioretinopathy  
2. Diabetic Retinopathy  
3. Disc Edema  
4. Glaucoma  
5. Healthy  
6. Macular Scar  
7. Myopia  
8. Pterygium  
9. Retinal Detachment  
10. Retinitis Pigmentosa  

---

## 🏗️ Model Architectures

### 🔹 DenseNet201 (Improved)
- ImageNet pretrained backbone  
- Gradual layer unfreezing  
- L2 regularization  
- Batch normalization and dropout  
- Excellent performance on fine-grained retinal features  

### 🔹 ConvNeXt (Improved)
- Modern convolutional neural network  
- Optimized fine-tuning strategy  
- Strong spatial feature extraction  
- Stable convergence  

### 🔹 Vision Transformer (ViT-B16 – Custom)
- Implemented from scratch in Keras  
- Patch embedding via Conv2D  
- Learnable class token  
- Positional embeddings  
- 12 Transformer encoder layers  
- AdamW optimizer with weight decay  
- Captures global retinal context  

---

## ⚙️ Training Configuration

---

## 📊 Performance Summary

### 🔬 Individual Model Performance

| Model | Accuracy | Precision | Recall |
|------|---------|----------|-------|
| DenseNet201 | **90.50%** | 90.77% | 90.13% |
| ConvNeXt | 79.65% | 81.39% | 77.30% |
| Vision Transformer (ViT-B16) | 66.74% | 79.23% | 48.48% |

---

### 🏆 Weighted Ensemble Performance

Optimized ensemble wei
| Metric | Score |
|------|------|
| **Accuracy** | **89.57%** |
| **ROC-AUC (avg)** | **0.9927** |
| **Macro F1-score** | **0.92** |
| **Weighted F1-score** | **0.90** |

The ensemble improves robustness and generalization by combining:
- DenseNet’s fine-grained feature extraction  
- ConvNeXt’s spatial modeling  
- ViT’s global contextual understanding  

---

## 📋 Detailed Classification Results (Ensemble)

| Class | Precision | Recall | F1-score |
|------|----------|-------|---------|
| Central Serous Chorioretinopathy | 0.89 | 0.88 | 0.89 |
| Diabetic Retinopathy | 0.98 | 0.96 | 0.97 |
| Disc Edema | 0.97 | 0.96 | 0.96 |
| Glaucoma | 0.86 | 0.79 | 0.82 |
| Healthy | 0.84 | 0.88 | 0.86 |
| Macular Scar | 0.86 | 0.85 | 0.85 |
| Myopia | 0.84 | 0.91 | 0.87 |
| Pterygium | 1.00 | 1.00 | 1.00 |
| Retinal Detachment | 0.98 | 1.00 | 0.99 |
| Retinitis Pigmentosa | 0.91 | 0.99 | 0.95 |

Overall Accuracy: **90%**  
Total Test Samples: **2446**

---

## 🧪 Evaluation Metrics
- Accuracy  
- Precision, Recall, F1-score  
- Confusion Matrix  
- ROC & AUC Curves (multi-class)  

---

## 📁 Project Structure
Ocular-disease-classification/
│
├── README.md
├── requirements.txt
├── train.py
├── evaluate.py
├── ensemble.py
│
├── models/
│ ├── densenet/
│ ├── convnext/
│ └── vit/
│
├── plots/
│ ├── confusion_matrices/
│ ├── roc_curves/
│ └── training_curves/
│
└── notebooks/
└── ocular_disease_training.ipynb



---

## 🩺 Clinical Relevance
The ensemble model demonstrates **excellent diagnostic performance** for vision-threatening conditions such as **Diabetic Retinopathy**, **Retinal Detachment**, and **Retinitis Pigmentosa**, making it suitable for automated screening and clinical decision-support systems.

---

## 🧬 Key Contributions
- Custom Vision Transformer implemented in pure Keras  
- Optimized class-weighted multiclass training  
- CNN–Transformer weighted ensemble  
- Exceptional ROC-AUC (0.9927)  
- Clinically meaningful per-class evaluation  

---

## 🔮 Future Work
- Explainable AI (Grad-CAM & attention maps)  
- Cross-dataset generalization  
- Real-time deployment (Streamlit / FastAPI)  
- Edge-device optimization  
- Federated learning for privacy-preserving AI  

---

## 🛠️ Technologies Used
- Python  
- TensorFlow / Keras  
- Keras-CV  
- NumPy, Pandas  
- Scikit-learn  
- Matplotlib, Seaborn  
- Google Colab (GPU)

---

## 👤 
**MOSES KIPRONO*  
College of Engineering, Physics, and Computing / The Catholic University of America 

---

## 📜 License
This project is licensed under the **MIT License**.
