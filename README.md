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
