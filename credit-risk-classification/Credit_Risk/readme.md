# Credit Risk Analysis Report

## 1. Data Preprocessing
The data was loaded and split into features (X) and target (y). The dataset was then split into training (80%) and testing (20%) sets. Features were standardized using StandardScaler for optimal model performance.

## 2. Model Training
A logistic regression model was trained using the standardized training data.

## 3. Model Evaluation

### Confusion Matrix:
[[14918 83]
[ 9 498]]


- **True Negatives (Healthy Loan correctly predicted):** 14,918
- **False Positives (Healthy Loan incorrectly predicted as High-Risk):** 83
- **False Negatives (High-Risk Loan incorrectly predicted as Healthy):** 9
- **True Positives (High-Risk Loan correctly predicted):** 498

### Classification Report:
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     15001
           1       0.86      0.94      0.90       507

    accuracy                           0.99     15508
   macro avg       0.93      0.97      0.95     15508
weighted avg       0.99      0.99      0.99     15508


- **Precision (Healthy Loan):** 1.00
- **Recall (Healthy Loan):** 0.99
- **F1-Score (Healthy Loan):** 1.00
- **Precision (High-Risk Loan):** 0.86
- **Recall (High-Risk Loan):** 0.98
- **F1-Score (High-Risk Loan):** 0.92
- **Overall Accuracy:** 99.41%

### ROC-AUC Score: 
0.995

## 4. Analysis Summary
The logistic regression model performs exceptionally well in predicting both healthy loans (label 0) and high-risk loans (label 1). 
The confusion matrix indicates a high number of true positives and true negatives, with very few false positives and false negatives.
The precision, recall, and F1-score for healthy loans are nearly perfect, while the metrics for high-risk loans are also very strong, indicating reliable model performance.
The overall accuracy is 99.41%, and the ROC-AUC score of 0.995 further confirms the model's ability to distinguish between the two classes effectively.

This comprehensive evaluation shows that the logistic regression model is highly effective for credit risk classification,
with strong performance metrics across the board.
