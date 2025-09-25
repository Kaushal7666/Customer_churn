# Customer Churn Prediction

This project focuses on predicting customer churn using various machine learning algorithms.  
The dataset was taken in **CSV format**, and several preprocessing and modeling steps were carried out.

---

## Dataset & Preprocessing
1. **Data Source**: CSV file (customer details with churn label).  
2. **Preprocessing Steps**:
   - Missing values handling
   - Encoding of categorical variables
   - Feature scaling (for numerical stability)

---

## Models Compared
We evaluated multiple machine learning models for churn prediction:

| Model               | Accuracy (%) |
|----------------------|--------------|
| Logistic Regression  | ~82.04       |
| Random Forest        | ~79.42       |
| XGBoost              | ~79.4        |

Additionally, ROC curve analysis was used to compare model performances.

---

## Why Logistic Regression Gave High Accuracy
Logistic Regression performed particularly well in this case due to:
- **Binary nature of the problem**: Churn prediction is a yes/no classification, which logistic regression is designed for.  
- **Linearly separable features**: Many customer behavior patterns might show linear relationships with churn probability.  
- **Less prone to overfitting**: Compared to complex models like Decision Tree or Random Forest, logistic regression is simpler and generalizes better when dataset size is moderate.  
- **Interpretability**: Logistic regression assigns weights to features, making important churn indicators easier to identify.
