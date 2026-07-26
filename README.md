# Metabolic Syndrome Prediction using Machine Learning

## Overview

This project develops and evaluates machine learning models to predict the risk of Metabolic Syndrome using structured clinical data. The workflow includes data preprocessing, feature engineering, missing value handling, categorical encoding, hyperparameter tuning, and comprehensive model evaluation.

Two classification algorithms—k-Nearest Neighbors (kNN) and Gaussian Naive Bayes—are implemented and compared using cross-validation and multiple evaluation metrics. The final model is optimized for ROC-AUC and generates prediction scores for unseen patient data.

---

## Objectives

- Preprocess and clean clinical data
- Handle missing values using KNN and statistical imputation
- Encode categorical variables
- Engineer clinically meaningful features
- Tune and compare multiple classification models
- Evaluate models using cross-validation and ROC-AUC
- Generate prediction scores for unseen data

---

## Machine Learning Pipeline

- Data preprocessing and cleaning
- Missing value imputation using KNNImputer and SimpleImputer
- Feature scaling using StandardScaler
- One-hot encoding of categorical variables
- Clinical feature engineering
- Stratified 10-fold cross-validation
- Hyperparameter tuning for kNN
- Model comparison using multiple evaluation metrics
- Final prediction generation

---

## Feature Engineering

Several domain-inspired features were engineered to improve predictive performance, including:

- RiskCount
- HighWaist
- HighTrig
- LowHDL
- HighGlucose
- TyG Index
- TG/HDL Ratio
- Glucose/HDL Ratio
- Lipid Accumulation Product (LAP)
- BMI × Waist Circumference
- Age × Uric Acid
- Log-transformed clinical variables

---

## Algorithms

- k-Nearest Neighbors (kNN)
- Gaussian Naive Bayes

---

## Model Evaluation

Models were evaluated using Stratified 10-Fold Cross-Validation and compared using:

- Accuracy
- Precision
- Recall
- Specificity
- F1-Score
- ROC-AUC
- Confusion Matrix
- ROC Curve

Hyperparameter tuning was performed for different values of **k** in the kNN classifier before selecting the final model.

---

## Technologies

- Python
- Scikit-learn
- Pandas
- NumPy
- Matplotlib

---

## Repository Structure

```text
├── dataset/
├── Metabolic_Syndrome_Prediction.ipynb
├── requirements.txt
└── README.md
```

---

## Results

The k-Nearest Neighbors classifier consistently outperformed Gaussian Naive Bayes during cross-validation and was selected as the final model. Feature engineering and careful preprocessing significantly improved predictive performance, while ROC-AUC was used as the primary evaluation metric for model selection.

---

## Author

**Yassin Zaki**
