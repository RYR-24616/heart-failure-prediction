# ❤️ Heart Failure Prediction using Machine Learning

A machine learning-based predictive system that estimates the risk of heart failure based on a patient’s medical attributes. The goal is to assist early intervention by predicting the likelihood of a cardiac event using reliable medical data.

## 🧠 Project Description

This project leverages supervised machine learning techniques to predict heart failure. It includes thorough data preprocessing, careful class proportion handling (especially for gender), model building using **XGBoost**, and detailed performance evaluation through metrics and visualizations.

Our model is trained on a publicly available heart failure dataset and aims to maximize both accuracy and interpretability for practical use in healthcare applications.

---

## ✅ Features

- Real-world dataset with gender-specific heart failure rates preserved (not artificially 50/50 balanced).
- Comprehensive preprocessing including:
  - One-hot encoding
  - Standard scaling
  - Controlled gender proportion for realism
- Model training using **XGBoost Classifier**
- Visualizations with `matplotlib` and `seaborn`
- Performance evaluated using:
  - Accuracy
  - Confusion Matrix
  - Classification Report

---

## 🔍 Problems Faced & Solutions Implemented

| Challenge | Solution |
|----------|----------|
| **Gender imbalance in dataset** | Instead of making it a strict 50-50 balance (which can distort reality), I adjusted the proportions while maintaining the original insight that **more males tend to die of heart failure**. This retained model realism. |
| **Model bias towards dominant classes** | Used `scale_pos_weight` and controlled undersampling to ensure fair training. |
| **Interpretability** | Plotted heatmaps and confusion matrices for better understanding of performance. |
| **Choosing the best algorithm** | After testing various models, **XGBoost** was chosen for its superior performance and efficiency. |

---

## 📈 Model Performance

- Accuracy: ✅ (Reported in notebook)
- Balanced handling of class distribution
- Strong ROC-AUC and precision scores

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn**
- **Scikit-learn**
- **XGBoost**

---

## 📁 Files

| File | Description |
|------|-------------|
| `Heart_disease.ipynb` | Full code with preprocessing, model training, evaluation |
| `README.md` | Project documentation |
| `heart.csv` | Dataset for the project | 


---
