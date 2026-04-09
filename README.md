# Readmission Risk Prediction

## Problem Statement

Hospital readmission remains a critical challenge in modern healthcare systems, contributing to increased medical costs, resource utilization, and patient health risks. Early identification of patients who are at a higher risk of readmission enables healthcare providers to take preventive actions and deliver personalized care.

This project focuses on analyzing comprehensive patient data—including demographic details, medical history, clinical conditions, and treatment outcomes—to predict the likelihood of hospital readmission. The primary objective is to assist healthcare professionals in identifying high-risk patients and implementing targeted interventions to reduce readmission rates.

## Model Training and Data Preparation

### Algorithms:
- **XGBoost**: Used for its ability to handle high-dimensional data efficiently and its strong performance on classification tasks.
- **Logistic Regression**: Applied with both **L1** (Lasso) and **L2** (Ridge) regularization to prevent overfitting and improve model generalization.

### Data Handling:
- **Data Split**: 80% of the data was used for training, and 20% for testing.
- **Preprocessing Steps**:
  - Handling missing values using appropriate imputation methods.
  - Normalizing data to ensure uniform scaling across features.
  - Feature engineering to enhance model performance by creating meaningful features.

### Ensemble Approach:
- An ensemble approach was employed by combining the strengths of XGBoost and Logistic Regression to improve the overall model performance.

- Comparative Analysis

A comprehensive comparative study was conducted to evaluate the performance of multiple machine learning and deep learning models.

Models Compared
XGBoost
CatBoost
Random Forest
Logistic Regression (L1 & L2)
RNN (Recurrent Neural Network)
LSTM (Long Short-Term Memory)
Hybrid Model Combinations

### Comparison Summary:

**Model	Strengths**	
**Limitations	Performance Insight**
-XGBoost	High accuracy, handles structured data well	Can overfit if not tuned	Best individual performer
-CatBoost	Handles categorical data efficiently	Slower training	Good but slightly lower than XGBoost
-Random Forest	Robust and reduces variance	Less efficient with large datasets	Moderate performance
-Logistic Regression (L1/L2)	Simple, interpretable, avoids overfitting	Limited for complex patterns	Stable baseline model
-RNN	Captures sequential patterns	Training complexity, vanishing gradient	Lower performance for tabular data
-LSTM	Better memory handling than RNN	Computationally expensive	Not ideal for this dataset
-Ensemble (XGBoost + Logistic Regression)	Combines strengths of models	Slight increase in complexity	Best overall performance (91%)

## Key Insight
Tree-based models outperformed deep learning models due to the structured/tabular nature of the dataset
The ensemble model provided the best balance between accuracy, generalization, and interpretability

## Evaluation and Metrics:
- **Metrics Used**:
  - Accuracy
  - Sensitivity (Recall)
  - Specificity
  - Precision
  - F1 Score
  - AUC-ROC
  - Confusion Matrix

- **Performance**:
  - Achieved **91% accuracy** in predicting hospital readmission risk.

## Evaluation and Results

- **Output**:
  - The model identifies high-risk and low-risk patients with their respective probability of readmission.
  
- **Root Cause Analysis**:
  - The system provides insights into potential causes for readmission for each patient based on the features contributing to the prediction.

## Deployment:
- The model was integrated into a frontend application, allowing for real-time predictions.
- The trained model was saved using **Pickle** for efficient reuse and future predictions.

## Risk Identification:
- The system highlights patients at risk and suggests tailored interventions to prevent readmissions.

## Dataset Link: https://datadryad.org/stash/dataset/doi:10.5061/dryad.70rxwdbxw
## procedure:
- create account on twillo and firebase and download the key as json and upload it in the folder.
- Run - dash_app.py to access the visulation on the patients reports
- run app_fin.py
for more queries message me on gmail: **dayanamuthu05@gmail.com**

