## Credit Card Fraud Detection:

## 📌 Overview
An end-to-end machine learning project for detecting fraudulent transactions using multiple classification models.
credit card fraud is a serious issue with highly imbalanced datasets. The goal of this project is to:

.Train & evaluate multiple ML classifiers
.Handle data imbalance using SMOTE
## Dataset
Source: https://www.kaggle.com/datasets/nelgiriyewithana/credit-card-fraud-detection-dataset-2023
Features: V1 to V28 and Amount
Target: Class (1 = Fraud, 0 = Not Fraud)

# The following classifiers were trained and evaluated:

"Logistic Regression"
"XGBoost"
"Decision Tree"
"Extra Trees"
"Naive Bayes"
"Random Forest"
"AdaBoost"

## 🧪 Evaluation Metrics (Each model was evaluated based on):
Precision, Recall, F1-Score
Confusion Matrix
ROC-AUC Curve

## 📊 Results Summary

| Model              | Accuracy | Precision | Recall | F1-Score | FP | FN |
|-------------------|----------|-----------|--------|----------|----|----|
| Logistic Regression | 0.998    | 1.00      | 1.00   | 1.00     | 58 | 137 |
| XGBoost           | 1.000    | 1.00      | 1.00   | 1.00     | 6  | 20  |
| Decision Tree     | 1.000    | 1.00      | 1.00   | 1.00     | 20 | 21  |
| Extra Trees       | 1.000    | 1.00      | 1.00   | 1.00     | 7  | 10  |
| Naive Bayes       | 0.932    | 0.98      | 0.88   | 0.93     | 1009 | 6697 |
| Random Forest     | 1.000    | 1.00      | 1.00   | 1.00     | 4  | 19  |
| AdaBoost          | 1.000    | 1.00      | 1.00   | 1.00     | 20 | 27  |


## 🔍 Detailed Model Analysis

### 1. **Logistic Regression**
- **Accuracy:** 99.8%
- **Confusion Matrix:** 
  - False Positives (FP): 58
  - False Negatives (FN): 137
- Slightly more false negatives than false positives. Performs well overall but not perfect.

---

### 2. **XGBoost**
- **Accuracy:** 100%
- **Confusion Matrix:** 
  - FP: 6
  - FN: 20
- Extremely high performance with very few misclassifications. One of the top-performing models.

---

### 3. **Decision Tree**
- **Accuracy:** 100%
- **Confusion Matrix:** 
  - FP: 20
  - FN: 21
- High accuracy but slightly more misclassifications than XGBoost or Random Forest.

---

### 4. **Extra Trees**
- **Accuracy:** 100%
- **Confusion Matrix:** 
  - FP: 7
  - FN: 10
- Performs similarly to Random Forest and XGBoost with minimal error.

---

### 5. **Naive Bayes**
- **Accuracy:** 93.2%
- **Confusion Matrix:** 
  - FP: 1009
  - FN: 6697
- Significantly lower performance. Assumptions of feature independence likely do not hold in this dataset.

---

### 6. **Random Forest**
- **Accuracy:** 100%
- **Confusion Matrix:** 
  - FP: 4
  - FN: 19
- Among the most accurate models with the least number of false positives.

---

### 7. **AdaBoost**
- **Accuracy:** 100%
- **Confusion Matrix:** 
  - FP: 20
  - FN: 27
- Performs well overall but slightly more errors compared to XGBoost and Random Forest.

---

## 📈 Conclusion

- **Best Performing Models:** XGBoost, Random Forest, Extra Trees — all achieved near-perfect accuracy with minimal false positives and false negatives.
- **Underperforming Model:** Naive Bayes — lower precision and recall due to its simplistic assumptions.
- **Recommendation:** For production deployment, **Random Forest** or **XGBoost** are the safest choices due to their consistent performance and low error rates.
