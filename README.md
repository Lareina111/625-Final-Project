# Predictive Analysis of Heart Disease Using Machine Learning

This repository contains the code and resources for a predictive analysis project aimed at identifying high-risk heart disease patients. The project utilizes machine learning techniques to analyze clinical indicators and predict the likelihood of heart disease.

## Authors
- Rong Ji
- Zeyue Zhang
- Chenxi Zhu
- Chuyi Yan

## Project Overview
Heart disease remains a leading cause of global mortality, accounting for approximately 32% of worldwide deaths. Early detection and prevention are critical for managing cardiovascular health. This project leverages machine learning to analyze clinical indicators and build predictive models that aid in identifying high-risk individuals.

## Data
The dataset is sourced from Kaggle's Sudden Cardiac Arrest dataset and includes medical records of 1,190 patients, with the following features:
- **Age**: Participant's age in years.
- **Sex**: Gender (1 = male, 0 = female).
- **Chest Pain Type**: Categories of chest pain.
- **Resting Blood Pressure**: Participant's resting blood pressure (mm Hg).
- **Cholesterol**: Serum cholesterol (mg/dl).
- **Fasting Blood Sugar**: Indicator for fasting blood sugar > 120 mg/dl.
- **Resting ECG**: Electrocardiogram results.
- **Max Heart Rate**: Maximum heart rate achieved.
- **Exercise-Induced Angina**: Presence of exercise-induced angina.
- **Oldpeak**: ST depression induced by exercise.
- **ST Slope**: Slope of the peak exercise ST segment.
- **Target**: Heart disease indicator (1 = yes, 0 = no).

## Methodology
### Data Preprocessing
1. **Missing Data Handling**:
   - Mean imputation for numerical variables.
   - Mode imputation for categorical variables.
   - Heatmaps used to visualize missing data patterns.

2. **Feature Engineering**:
   - Standardization of continuous features.
   - Polynomial features to capture non-linear interactions.
   - Feature selection using Random Forest importance metrics.

### Model Training and Evaluation
Machine learning models were trained and evaluated using stratified train-test splits (70:30). Models included:
- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)
- XGBoost
- K-Nearest Neighbors (KNN)
- Gradient Boosting

Evaluation metrics:
- Accuracy
- Precision, Recall, F1-score
- ROC-AUC

## Results
- **Best Model**: XGBoost
  - **Accuracy**: 91.3%
  - **ROC-AUC**: 95.1%
- Random Forest and Gradient Boosting also performed well, with high accuracy and generalizability.

## Conclusion
Machine learning models, especially ensemble methods like XGBoost and Random Forest, demonstrated excellent potential for predicting heart disease. Future work includes addressing missing data biases, enhancing feature availability, and optimizing models for real-time clinical use.

## Repository Contents
- `data/`: Dataset files.
- `notebooks/`: Jupyter notebooks with preprocessing, modeling, and evaluation.
- `src/`: Python scripts for data processing and model training.
- `results/`: Model performance metrics and visualizations.
- `README.md`: Project documentation.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo-name.git
   cd your-repo-name
