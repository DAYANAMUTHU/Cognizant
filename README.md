Readmission Risk Prediction
Problem Statement

Hospital readmission is a significant concern for healthcare systems, leading to increased costs and patient complications. Accurately predicting which patients are at higher risk of readmission can enable healthcare providers to proactively offer personalized care and reduce the likelihood of readmission. This project aims to analyze comprehensive patient data, including demographics, medical history, vital signs, and treatment outcomes, to predict the risk of hospital readmission. The goal is to equip healthcare providers with predictive insights, allowing them to identify high-risk individuals and develop personalized care plans that prevent potential readmissions.

Model Training and Data Preparation
Algorithms:
XGBoost: Used for its ability to handle high-dimensional data efficiently and its strong performance on classification tasks.
Logistic Regression: Applied with both L1 (Lasso) and L2 (Ridge) regularization to prevent overfitting and improve model generalization.
CatBoost: Utilized for handling categorical features effectively with minimal preprocessing.
Random Forest: Applied for its robustness and ability to reduce variance through ensemble learning.
RNN (Recurrent Neural Network): Explored for sequential pattern learning in patient data.
LSTM (Long Short-Term Memory): Used to capture long-term dependencies in sequential healthcare data.
Data Handling:
Data Split: 80% of the data was used for training, and 20% for testing.
Preprocessing Steps:
Handling missing values using appropriate imputation methods
Normalizing data to ensure uniform scaling across features
Feature engineering to enhance model performance by creating meaningful features
Ensemble Approach:
An ensemble approach was employed by combining the strengths of XGBoost and Logistic Regression to improve the overall model performance and generalization capability.
Comparative Analysis
A comparative study was conducted using multiple machine learning and deep learning models to evaluate their effectiveness in predicting hospital readmission.
Models Used:
XGBoost
CatBoost
Random Forest
Logistic Regression (L1 & L2)
RNN
LSTM
Hybrid Model Combinations
Observations:
XGBoost achieved the highest performance among individual models due to its efficiency with structured data.
CatBoost performed well with categorical features but showed slightly lower accuracy compared to XGBoost.
Random Forest provided stable results but was less efficient on large datasets.
Logistic Regression offered strong interpretability and served as a reliable baseline model.
RNN and LSTM showed lower performance as the dataset is tabular rather than sequential in nature.
The ensemble model (XGBoost + Logistic Regression) outperformed all individual models by achieving better balance between bias and variance.
Evaluation and Metrics:
Metrics Used:
Accuracy
Sensitivity (Recall)
Specificity
Precision
F1 Score
AUC-ROC
Confusion Matrix
Performance:
Achieved 91% accuracy in predicting hospital readmission risk
The ensemble model demonstrated improved generalization and balanced classification performance
Evaluation and Results
Output:
The model identifies high-risk and low-risk patients with their respective probability of readmission
Root Cause Analysis:
The system provides insights into potential causes for readmission for each patient based on the most influential features contributing to the prediction
Deployment:
The model was integrated into a frontend application, allowing for real-time predictions
The trained model was saved using Pickle for efficient reuse and future predictions
Risk Identification:
The system highlights patients at risk
Provides tailored recommendations and preventive interventions to reduce readmission rates
Dataset Link:

https://datadryad.org/stash/dataset/doi:10.5061/dryad.70rxwdbxw

Procedure:
Create an account on Twilio and Firebase, then download the key in JSON format and upload it into the project folder
Run dash_app.py to access the visualization of patient reports
Run app_fin.py for executing additional queries
Contact:

For more queries, message via email:
dayanamuthu05@gmail.com
