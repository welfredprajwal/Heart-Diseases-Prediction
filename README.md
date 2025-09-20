# Heart-Diseases-Prediction-Random Forest

# Overview

This project predicts the presence of heart disease in patients using a Random Forest classifier. Heart disease is one of the leading causes of mortality worldwide, and early prediction can help in timely intervention and treatment.

The dataset includes clinical and demographic features that are commonly used for diagnosing heart conditions. By leveraging these features, the model predicts whether a patient has heart disease (target = 1) or not (target = 0).

# Dataset

| Feature  | Description                                                              |
| -------- | ------------------------------------------------------------------------ |
| age      | Age of the patient in years                                              |
| sex      | Gender of the patient (1 = male, 0 = female)                             |
| cp       | Chest pain type (0–3)                                                    |
| trestbps | Resting blood pressure (mm Hg)                                           |
| chol     | Serum cholesterol (mg/dl)                                                |
| fbs      | Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)                    |
| restecg  | Resting electrocardiographic results (0–2)                               |
| thalach  | Maximum heart rate achieved                                              |
| exang    | Exercise-induced angina (1 = yes, 0 = no)                                |
| oldpeak  | ST depression induced by exercise relative to rest                       |
| slope    | Slope of the peak exercise ST segment (0–2)                              |
| ca       | Number of major vessels (0–3) colored by fluoroscopy                     |
| thal     | Thalassemia (1 = normal, 2 = fixed defect, 3 = reversible defect)        |
| target   | Diagnosis of heart disease (1 = presence, 0 = absence) – target variable |

# Why Random Forest?

Ensemble Learning Algorithm: Combines multiple decision trees to improve accuracy.
Handles Non-linearity: Captures complex relationships between features.
Reduces Overfitting: Aggregating multiple trees reduces variance.
Feature Importance: Identifies key predictors of heart disease.

# Project Workflow

1.Data Preprocessing

  Handle missing values and outliers
  Encode categorical variables (if needed)
  Feature scaling (optional for tree-based models)

2.Exploratory Data Analysis (EDA)

  Analyze distributions of clinical features
  Visualize correlations to identify key predictors
  Understand patient demographics and risk factors

3.Random Forest Model Training

  Split data into training and testing sets
  Train Random Forest classifier
  Tune hyperparameters (number of trees, max depth, min samples split) using GridSearchCV
  
4.Model Evaluation

Evaluate using metrics such as:
Accuracy,Precision,Recall,F1-Score,Confusion Matrix,ROC-AUC

5.Prediction

Predict heart disease presence for new patients
Identify high-risk patients for early intervention

# Results

Metric	Score
Accuracy	~85–92% (depending on dataset split and preprocessing)

