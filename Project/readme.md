# 🩺 Melanoma Detection Using Convolutional Neural Networks  

## 📌 Project Overview  
This project focuses on enhancing **melanoma detection** using **Convolutional Neural Networks (CNNs)**. The study replicates and improves the methodology from the paper **"Melanoma Detection Using Regular Convolutional Neural Networks"** by **Aya Abu Ali and Hasan Al-Marzouqi**.  

Melanoma is one of the most **aggressive types of skin cancer**, and early detection is critical. This project aims to develop an **automated CNN model** that surpasses the diagnostic accuracy of dermatologists (75-85%).  

---

## 🏗 Project Objectives  
✅ **Replicate** the CNN model from the original research paper and evaluate its performance.  
✅ **Improve sensitivity and accuracy** by modifying the CNN architecture and preprocessing techniques.  
✅ **Compare performance** between different models and datasets.  
✅ **Achieve at least 85% accuracy** to outperform human dermatologists.  

---

## 📂 Datasets Used  

### **1️⃣ ISBI Challenge 2016 Dataset**  
- Contains **900 training images** and **379 test images**.  
- Unbalanced dataset (more benign than malignant cases).  
- Applied **oversampling, undersampling, and class weighting** to address imbalance.  

### **2️⃣ HAM10000 Dataset (Human Against Machine)**  
- Published by the **National Library of Medicine**.  
- Contains **10,015 high-quality dermatoscopic images** collected over 20 years.  
- Well-balanced dataset with **equal benign and malignant samples**.  

👉 **Switching to the HAM10000 dataset led to significantly better results.**  

---

## 🏗 Model Architecture  

### **1️⃣ Replicated CNN from Original Paper**  
- 5 convolutional blocks  
- Different kernel sizes (5x5, 4x4, 1x1)  
- Accuracy: **81.6%**  
- **Weakness:** High specificity (98%) but very low sensitivity (**14.9%** → many false negatives).  

### **2️⃣ Improved CNN Model**  
✅ Increased to **6 convolutional blocks** for deeper feature extraction.  
✅ Standardized **3x3 kernels** in all layers for better generalization.  
✅ Added **batch normalization** and **data augmentation** (random flip & rotation).  
✅ Removed **dropout layers**, improving model stability.  
✅ Accuracy: **88%**, significantly reducing false negatives.  

---

## 📊 Model Training & Evaluation  

### **Loss Function & Optimization**  
- **Cross-entropy loss function** for binary classification.  
- **Adam optimizer** with an initial learning rate of **0.001**.  

### **Performance Metrics**  
📌 **Original CNN (ISBI Dataset):**  
- Accuracy: **81.6%**  
- Specificity: **98%**  
- Sensitivity: **14.9%** ❌ (Many false negatives)  

📌 **Improved CNN (HAM10000 Dataset):**  
- Accuracy: **88%** ✅  
- Sensitivity: **Significantly improved** (Lower false negatives)  
- **Surpasses dermatologist accuracy (75-85%)** ✅  

### **Confusion Matrix Analysis**  
- Original CNN **missed 125 melanoma cases** (false negatives).  
- Improved CNN **reduced false negatives to 73** → **safer model for medical diagnosis**.  

---


