# 🩺 Melanoma Detection Using Convolutional Neural Networks (CNNs)

This repository contains a **deep learning project for detecting melanoma (skin cancer)** using **Convolutional Neural Networks**, inspired by the work of Aya Abu Ali and Hasan Al-Marzouqi. The goal is to replicate and improve upon their model for **benign vs. malignant skin lesion classification** using dermatoscopic images.

---

## 📌 Features & Concepts Covered

✔ Implementation of **two CNN architectures**: one based on the original paper and a new, improved version.  
✔ Use of two public datasets: **ISBI 2016** and **HAM10000** for training and evaluation.  
✔ **Image preprocessing and data augmentation** techniques to boost model generalization.  
✔ Balanced vs. unbalanced dataset strategies: oversampling, undersampling, and class weighting.  
✔ **Binary classification** using softmax and cross-entropy loss.  
✔ Model evaluation using **accuracy, sensitivity, specificity**, and **confusion matrix**.  
✔ Use of **TensorFlow and Keras** for model development.  
✔ Thorough **comparison of original vs. improved CNN performance**.

---

## 📘 Theory Overview

This project addresses the difficulty of accurately diagnosing **melanoma**, a dangerous form of skin cancer. The paper we replicate highlights the shortcomings of their model, such as **low sensitivity**. Our enhancements focus on:

- Building a **deeper CNN with better kernel and pooling strategies**.
- Removing dropout and relying on **data augmentation** instead.
- Using **balanced datasets** to reduce bias and false negatives.
- Applying standard **binary classification loss**: categorical cross-entropy.

---

## 📊 Results Summary

| Model         | Dataset     | Accuracy | Sensitivity | Specificity |
|---------------|-------------|----------|-------------|-------------|
| Original CNN  | ISBI 2016   | 81.6%    | 14.9%       | 98%         |
| Improved CNN  | HAM10000    | 88.0%    | 85.2%       | 90.1%       |

---

## 📈 F1 Score Comparison

The F1 score balances precision and recall, and it's especially useful for evaluating models with imbalanced data.  
- **Original CNN F1 Score**: ~25%  
- **Improved CNN F1 Score**: ~87%  

---

## 🧠 Technologies Used

- Python, Jupyter Notebooks  
- TensorFlow + Keras  
- Pandas, NumPy, Matplotlib  
- Data augmentation techniques (Keras layers)  
- Balanced datasets (oversampling, undersampling)

---

## 🙌 Contributors

- **Antonio Castañares** – MSc in Computer Science @ Illinois Tech  
- **Nicolás Corsini** – MSc in Computer Science @ Illinois Tech
