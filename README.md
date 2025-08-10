# 💳 Fraud Transaction Detection using Machine Learning

## 📌 Overview
This project implements a **fraud detection model** to classify banking transactions as *fraudulent* or *non-fraudulent*.  
It leverages machine learning techniques, data preprocessing, and **Random Forest Classifier** with class imbalance handling to improve detection accuracy.

---

## ✨ Features
- Data preprocessing: handling missing values, encoding categorical features, and scaling.
- **SMOTE** for handling imbalanced datasets.
- **Random Forest Classifier** for fraud prediction.
- Performance evaluation using:
  - Classification Report (Precision, Recall, F1-score)
  - Confusion Matrix
  - ROC-AUC Score
- Function to predict fraud for a **new transaction input**.

---

## 🛠 Tech Stack
- **Programming Language:** Python 3.x
- **Libraries:**
  - pandas, numpy – Data manipulation
  - scikit-learn – Model training and evaluation
  - imbalanced-learn (SMOTE) – Handling class imbalance
  - seaborn, matplotlib – Data visualization

---

## 📂 Project Workflow
1. **Load Dataset**  
   Reads the `Fraud.csv` dataset containing transaction records.

2. **Data Cleaning & Preprocessing**
   - Remove unnecessary ID columns (`nameOrig`, `nameDest`).
   - Encode `type` column using One-Hot Encoding.
   - Handle missing values.
   - Scale features with **StandardScaler**.

3. **Handling Class Imbalance**
   - Apply **SMOTE** to balance the fraud/non-fraud classes.

4. **Model Training**
   - Train a **Random Forest Classifier** on preprocessed data.

5. **Model Evaluation**
   - Check model performance using metrics & visualizations.

6. **Custom Prediction Function**
   - Accepts transaction details as input and returns `"Fraud"` or `"Not Fraud"`.

---
