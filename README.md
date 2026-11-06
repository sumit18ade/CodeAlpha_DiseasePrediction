# 🩺 Disease Prediction from Medical Data

A Machine Learning project developed as part of the **CodeAlpha Machine Learning Internship – Task 4**.

The project predicts the possibility of selected diseases using structured medical data and multiple classification algorithms.

---


## 🎯 Objective

Predict the possibility of diseases based on patient and medical data using supervised machine learning classification techniques.

The project covers three medical prediction problems:

- ❤️ Heart Disease Prediction
- 🩸 Diabetes Prediction
- 🎗️ Breast Cancer Prediction

---

## 🚀 Key Features

- Patient data based disease prediction
- Structured medical dataset processing
- Data preprocessing and missing-value handling
- Multiple classification algorithms
- Model performance comparison
- Accuracy, Precision, Recall and F1-score evaluation
- ROC-AUC evaluation
- Confusion Matrix visualization
- ROC Curve visualization
- Interactive Streamlit web application
- Separate prediction interfaces for each disease
- Saved trained machine learning pipelines

---

## 🧠 Machine Learning Algorithms

The project implements four classification algorithms:

### 1. Logistic Regression
A linear classification algorithm used to estimate the probability of a binary outcome.

### 2. Support Vector Machine (SVM)
A supervised learning algorithm that finds an optimal decision boundary between classes.

### 3. Random Forest
An ensemble learning algorithm that combines multiple decision trees for classification.

### 4. XGBoost
A gradient boosting algorithm designed for efficient and accurate classification.

---

## 📊 Datasets

### ❤️ Heart Disease

Dataset based on the **UCI Heart Disease dataset**.

Features include:

- Age
- Sex
- Chest pain type
- Resting blood pressure
- Serum cholesterol
- Fasting blood sugar
- Resting ECG
- Maximum heart rate
- Exercise-induced angina
- ST depression
- ST slope
- Number of major vessels
- Thalassemia-related measurement

The target represents the presence or absence of heart disease.

---

### 🩸 Diabetes

Dataset based on the **Pima Indians Diabetes dataset**.

Features include:

- Pregnancies
- Glucose
- Blood Pressure
- Skin Thickness
- Insulin
- BMI
- Diabetes Pedigree Function
- Age

The target represents the diabetes outcome.

---

### 🎗️ Breast Cancer

Dataset based on the **Breast Cancer Wisconsin (Diagnostic) dataset**.

The dataset contains diagnostic measurements derived from breast mass characteristics, including:

- Mean measurements
- Standard error measurements
- Worst measurements

The target represents malignant or non-malignant diagnosis classes.

---

## 📈 Model Evaluation

Each model is evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

The project also generates:

- Confusion Matrix
- ROC Curves
- Model comparison results

---

## 📊 Model Results

### ❤️ Heart Disease

| Model | Accuracy | Precision | Recall | F1 | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 86.89% | 81.25% | 92.86% | 86.67% | 95.13% |
| SVM | 85.25% | 80.65% | 89.29% | 84.75% | 94.37% |
| Random Forest | 91.80% | 87.10% | 96.43% | 91.53% | 95.78% |
| XGBoost | 88.52% | 81.82% | 96.43% | 88.52% | 94.91% |

### 🩸 Diabetes

| Model | Accuracy | Precision | Recall | F1 | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 70.78% | 60.00% | 50.00% | 54.55% | 81.30% |
| SVM | 74.03% | 65.22% | 55.56% | 60.00% | 79.64% |
| Random Forest | 74.03% | 65.91% | 53.70% | 59.18% | 81.60% |
| XGBoost | 75.32% | 65.38% | 62.96% | 64.15% | 83.00% |

### 🎗️ Breast Cancer

| Model | Accuracy | Precision | Recall | F1 | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 96.49% | 97.50% | 92.86% | 95.12% | 99.60% |
| SVM | 97.37% | 100.00% | 92.86% | 96.30% | 99.47% |
| Random Forest | 97.37% | 100.00% | 92.86% | 96.30% | 99.44% |
| XGBoost | 96.49% | 100.00% | 90.48% | 95.00% | 99.47% |

---

## 🛠️ Technologies Used

### Programming Language
- Python

### Machine Learning
- Scikit-learn
- XGBoost

### Data Processing
- Pandas
- NumPy

### Visualization
- Matplotlib
- Seaborn

### Web Application
- Streamlit

### Model Persistence
- Joblib

### Dataset Access
- UCI ML Repository
- Scikit-learn datasets

---

## 📁 Project Structure

```text
CodeAlpha_DiseasePrediction/
│
├── data/
│   └── diabetes.csv
│
├── models/
│   ├── heart_logistic_regression.joblib
│   ├── heart_svm.joblib
│   ├── heart_random_forest.joblib
│   ├── heart_xgboost.joblib
│   ├── diabetes_logistic_regression.joblib
│   ├── diabetes_svm.joblib
│   ├── diabetes_random_forest.joblib
│   ├── diabetes_xgboost.joblib
│   ├── breastcancer_logistic_regression.joblib
│   ├── breastcancer_svm.joblib
│   ├── breastcancer_random_forest.joblib
│   ├── breastcancer_xgboost.joblib
│   └── breastcancer_features.json
│
├── screenshots/
│   ├── heart_*.png
│   ├── diabetes_*.png
│   └── breastcancer_*.png
│
├── src/
│   ├── common.py
│   ├── train_heart.py
│   ├── train_diabetes.py
│   ├── train_breast_cancer.py
│   └── train_all.py
│
├── app/
│   └── app.py
│
├── README.md
├── requirements.txt
├── .gitignore
└── run.ps1
