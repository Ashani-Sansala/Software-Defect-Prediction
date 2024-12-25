# Software-Defect-Prediction

This project focuses on predicting software defects using ensemble approach in ML. This includes data preprocessing, exploratory data analysis, model training and testing, hyperparameter tuning, and an ensemble model to improve prediction accuracy.

---

## Features

- Data preprocessing with the handling of missing values, outlier retention, data transformation, and feature scaling.
- Imbalanced dataset handling using SMOTE (Synthetic Minority Oversampling Technique).
- Three machine learning models: **XGBoost**, **LightGBM**, and **Random Forest**.
- Hyperparameter tuning using **GridSearchCV**.
- Stacking ensemble model for enhanced prediction accuracy.
- Comprehensive evaluation metrics, including accuracy, F1 score, ROC-AUC, confusion matrix, and classification reports.

## Dataset

The project uses the **JM1 dataset**, which is part of the NASA Metrics Data Program (MDP). This dataset contains real-world metrics from a NASA software system and is commonly used for defect prediction research.

- **Dataset Features**:
  - Includes various code metrics such as lines of code, cyclomatic complexity, and Halstead metrics.
  - This contains 22 attributes and 10885 instances.
  - The target variable indicates whether a software module is defective (`1`) or non-defective (`0`).

You can download the JM1 dataset from the [kaggle](https://www.kaggle.com/datasets/semustafacevik/software-defect-prediction/data).

## Model Description
The Stacking Ensemble combines predictions from three base models using Logistic Regression as the meta model:
- **XGBoost**: Extreme Gradient Boosting, a gradient-boosted decision tree model.
- **LightGBM**: A highly efficient gradient-boosted framework optimized for speed and performance.
- **Random Forest**: An ensemble learning method using multiple decision trees.

## Evaluation Results

### Evaluation results of each base model:
![Screenshot 2024-12-22 103042](https://github.com/user-attachments/assets/d1f63deb-c1e1-45d7-b50f-f2a7cf92fcc8)
![image](https://github.com/user-attachments/assets/78f4c603-63c1-45d7-abeb-a3f284086ddf)

### Evaluation results of stacking ensemble:
- Accuracy: 0.89
- ROC-AUC Score: 0.95
