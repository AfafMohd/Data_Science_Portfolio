# 🩺 Diabetes Classification using Machine Learning

This project focuses on predicting diabetes using the **Pima Indians Diabetes dataset** through a complete machine learning pipeline including:

- Exploratory Data Analysis (EDA)
- Missing value handling
- Outlier detection and treatment
- Feature engineering
- Data visualization
- Model building and hyperparameter tuning
- Ensemble learning (Voting Classifier)

---

## 📌 Dataset

The dataset contains medical records of 768 women aged 21 and above.

### Target Variable:
- `Outcome`
  - 0 → Non-Diabetic  
  - 1 → Diabetic  

### Features:
- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age

---

## 🔍 Exploratory Data Analysis (EDA)

### Key Steps:
- Dataset inspection using `check_df()`
- No missing values initially, but **zero values treated as missing**
- Columns corrected:
  - Glucose
  - BloodPressure
  - SkinThickness
  - Insulin
  - BMI

### Insight:
Zero values were not valid medical values → treated as missing and imputed.

---

## 🧹 Data Preprocessing

### 1. Missing Value Handling
- Converted invalid 0 values → NaN
- Imputed using **median grouped by Outcome**

### 2. Outlier Handling
- Detected using IQR method
- Applied **winsorization (capping method)** instead of removal

### 3. Feature Scaling
- Used `RobustScaler` (handles outliers well)

---

## 🧠 Feature Engineering

Created new medical risk-based features:

- `Insulin_CAT`
- `BloodPressure_CAT`
- `Glucose_CAT`
- `BMI_CAT`
- `Age_CAT`
- `Life_Level_CAT`

These features improved interpretability and model performance.

---

## 📊 Visualization

- Boxplots for outlier analysis
- Histograms before vs after preprocessing
- Diabetes distribution (class imbalance check)
- Category-wise diabetes analysis

### Key Insight:
- Glucose, BMI, and Insulin show strong separation between classes

---

## 🤖 Machine Learning Models

Models used:

- Logistic Regression
- Decision Tree (CART)
- Random Forest
- Gradient Boosting
- XGBoost
- LightGBM

---

## 🚀 Baseline Model Performance (Before Preprocessing)

| Model        | Accuracy |
|--------------|----------|
| LR           | 0.7671   |
| KNN          | 0.7182   |
| CART         | 0.7296   |
| RF           | 0.7703   |
| GBM          | 0.7654   |
| XGBoost      | 0.7524   |
| LightGBM     | 0.7378   |

---

## ⚙️ After Preprocessing

- Missing value treatment
- Outlier handling
- Feature engineering
- Scaling

### Best Models:

| Model     | Accuracy |
|-----------|----------|
| RF        | 0.8926   |
| XGBoost   | 0.8958   |
| LightGBM  | 0.8942   |

---

## 🔧 Hyperparameter Tuning Results

| Model      | Best Accuracy |
|------------|--------------|
| CART       | 0.8616       |
| RF         | 0.8779       |
| XGBoost    | 0.9088       |
| LightGBM   | 0.9023       |

---

## 🏆 Final Ensemble Model

### Voting Classifier (Soft Voting)

- Accuracy: **0.8925**
- F1 Score: **0.8421**
- ROC AUC: **0.9516**

---

## 📈 Feature Importance

Top influential features:

- Glucose
- BMI
- Insulin

These are the strongest predictors of diabetes.

---

## 📊 Model Evaluation (Best Model: LightGBM)

### Classification Report:
- Accuracy: **0.87**
- Class 0 (Non-Diabetic): Strong precision and recall
- Class 1 (Diabetic): Slightly lower recall (missed cases)

---

## 📉 Confusion Matrix

- TP: Correct diabetic detection
- TN: Correct non-diabetic detection
- FP: False alarms
- FN: Missed diabetic cases

---

## 📌 Conclusion

This project demonstrates a full end-to-end ML pipeline:

✔ Data Cleaning (handling invalid zeros)  
✔ Missing Value Imputation  
✔ Outlier Treatment  
✔ Feature Engineering  
✔ Model Comparison  
✔ Hyperparameter Tuning  
✔ Ensemble Learning  

### 🔑 Key Finding:
- **Glucose, BMI, and Insulin are the most important predictors**
- **LightGBM & XGBoost performed best overall**
- Preprocessing significantly improved model performance

---

## 🚀 Tools & Libraries

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- XGBoost
- LightGBM
