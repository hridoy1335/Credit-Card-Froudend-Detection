# Credit Card Fraud Detection Model

## Description
This project implements a machine learning model to detect credit card fraud. The model identifies fraudulent transactions using the Credit Card Fraud Detection dataset from Kaggle. Given the severe class imbalance, techniques like SMOTE and appropriate evaluation metrics (e.g., recall, ROC-AUC) are employed to ensure robust performance.

## Dataset
- **Source**: [Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- **Features**:  
  - 28 anonymized features (V1-V28) from PCA transformation.
  - `Time` (seconds elapsed between transactions).
  - `Amount` (transaction value).
  - `Class` (target: 0 = legitimate, 1 = fraudulent).
- **Class Distribution**:  
  - 99.83% legitimate (284,315 samples).
  - 0.17% fraudulent (492 samples).

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/hridoy1335/Credit-Card-Froudend-Detection/
   cd credit-card-fraud-detection
   
## Installation required library
2. pip install -r requirements.txt
   pandas
   numpy
   scikit-learn
   imbalanced-learn
   joblib

Data Preprocessing

Class Imbalance Handling: Apply SMOTE to oversample the minority class.
Feature Scaling: Use StandardScaler to normalize Time and Amount.
Train-Test Split: 80% training, 20% testing with stratified sampling.
Model Development

Algorithms

XGBoost (final model due to highest recall).
Logistic Regression (baseline).
Random Forest.

Future Improvements

Experiment with deep learning (autoencoders for anomaly detection).
Integrate real-time transaction scoring.
Develop feature engineering pipelines (e.g., transaction frequency).
Implement model explainability tools (SHAP, LIME).
