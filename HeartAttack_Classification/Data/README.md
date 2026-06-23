# 🫀 Heart Disease Classification Project

## 📌 Project Overview
This project focuses on predicting the presence of heart disease using machine learning classification models. The dataset contains patient medical attributes such as age, cholesterol levels, chest pain type, and ECG results.

The goal is to build a model that can accurately classify whether a patient is at risk of heart disease.

---

## 📊 Dataset Description

The dataset used is `heart.csv`, which contains clinical and diagnostic features collected from patients.

### 🔑 Features

| Feature | Description |
|--------|-------------|
| age | Age of the patient |
| sex | Gender (1 = male, 0 = female) |
| cp | Chest pain type (0–3) |
| trestbps | Resting blood pressure (mm Hg) |
| chol | Serum cholesterol (mg/dl) |
| fbs | Fasting blood sugar > 120 mg/dl (1 = true, 0 = false) |
| restecg | Resting electrocardiographic results |
| thalach | Maximum heart rate achieved |
| exang | Exercise induced angina (1 = yes, 0 = no) |
| oldpeak | ST depression induced by exercise |
| slope | Slope of peak exercise ST segment |
| ca | Number of major vessels (0–3) colored by fluoroscopy |
| thal | Thalassemia type (0 = normal, 1 = fixed defect, 2 = reversible defect) |

### 🎯 Target Variable
| Feature | Description |
|--------|-------------|
| target | 0 = no heart disease, 1 = heart disease present |

---

## ⚙️ Machine Learning Workflow

1. Data loading and exploration
2. Data preprocessing
3. Feature analysis and visualization
4. Train-test split
5. Model training (e.g., Logistic Regression, Random Forest, XGBoost, etc.)
6. Model evaluation using accuracy, ROC-AUC, confusion matrix

---

## 📈 Evaluation Metrics

- Accuracy
- Precision & Recall
- F1-score
- ROC-AUC Curve

---

## 🧠 Models Used

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- Gradient Boosting
- XGBoost
- LightGBM

---

## 🚀 Results

Best performing model is selected based on ROC-AUC score and accuracy.

---

## 📂 Dataset Source

Commonly used heart disease dataset from UCI Machine Learning Repository / Kaggle.

---

## 📌 Future Improvements

- Hyperparameter tuning
- Feature engineering
- Handling class imbalance
- Deployment as a web app (Streamlit / Flask)

---

