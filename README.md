
## 📌 Overview fo project
An end-to-end machine learning project for detecting fraudulent transactions using multiple classification models.
The goal of this project is to Train & evaluate multiple ML classifiers
 
## Dataset

# Source: 

https://www.kaggle.com/datasets/nelgiriyewithana/credit-card-fraud-detection-dataset-2023.

# Features: 

V1 to V28 and Amount

# Target: 

Class (1 = Fraud, 0 = Not Fraud)

The following classifiers were trained and evaluated:

# "Logistic Regression"

# "XGBoost"

# "Decision Tree"  

# "Extra Trees"

# "Naive Bayes"

# "Random Forest"

# "AdaBoost"

## 🧪 Evaluation Metrics (Each model was evaluated based on):

Precision, Recall, F1-Score, Confusion Matrix, ROC-AUC Curve

## ✅ Results Summary

| Model              | Accuracy | Precision (1) | Recall (1) | F1-Score (1) |
|-------------------|----------|---------------|------------|--------------|
| Logistic Regression | 96.5%   | 0.98          | 0.95       | 0.96         |
| XGBoost             | 100%    | 1.00          | 1.00       | 1.00         |
| Decision Tree       | 99.8%   | 1.00          | 1.00       | 1.00         |
| Extra Trees         | 100%    | 1.00          | 1.00       | 1.00         |
| Naive Bayes         | 91.9%   | 0.98          | 0.86       | 0.91         |
| Random Forest       | 100%    | 1.00          | 1.00       | 1.00         |
| AdaBoost            | 96.3%   | 0.97          | 0.95       | 0.96         |


## 🔍 Detailed Model Analysis

### 1. **Logistic Regression**

Logistic Regression

Accuracy: 96.5%

Precision: 0.97 (macro avg)

Recall: 0.96 (macro avg)

F1-score: 0.96 (macro avg)

Remarks: Performs well with balanced precision and recall. Some misclassifications present.


### 2. XGBoost

Accuracy: 100%

Precision/Recall/F1: 1.00 (all metrics)

Remarks: Near-perfect classification with almost no errors.

### 3. Decision Tree

Accuracy: 99.8%

Precision/Recall/F1: 1.00 (all metrics)

Remarks: Extremely high accuracy, very few misclassifications.

### 4. Extra Trees

Accuracy: 100%

Precision/Recall/F1: 1.00 (all metrics)

Remarks: Outstanding performance, almost perfect classification.

### 5. Naive Bayes

Accuracy: 91.9%

Precision: 0.93 (macro avg)

Recall: 0.92 (macro avg)

F1-score: 0.92 (macro avg)
 
Remarks: Lower performance compared to tree-based models, especially for class 1.

### 6. Random Forest

Accuracy: 100%

Precision/Recall/F1: 1.00 (all metrics)

Remarks: Excellent performance, virtually no misclassifications.

### 7. AdaBoost

Accuracy: 96.3%

Precision: 0.96 (macro avg)

Recall: 0.96 (macro avg)

F1-score: 0.96 (macro avg)

Remarks: Comparable to Logistic Regression, with some misclassifications.

## 📝 Conclusion

Best Performers: XGBoost, Extra Trees, and Random Forest achieved perfect or near-perfect accuracy, precision, recall, and F1-scores, making them the top choices for this dataset.

Strong Classical Models: Decision Tree also performed exceptionally well, with only a handful of misclassifications.

Baseline Models: Logistic Regression and AdaBoost performed well, but not as well as the ensemble/tree-based methods.

Naive Bayes: This model lagged behind others, particularly in recall for class 1, indicating it's less suited for this dataset.

Recommendation: For deployment or further analysis, XGBoost, Extra Trees, or Random Forest are recommended due to their superior performance.


