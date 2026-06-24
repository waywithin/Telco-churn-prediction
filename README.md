## Telco Customer Churn Prediction

### Project Overview

- This project focuses on predicting customer churn in the telecommunications industry using machine learning techniques. 
- The goal is to identify customers who are likely to discontinue the service, allowing businesses to take proactive retention measures.

---

### Dataset

The model was trained and evaluated using a publicly available telecom customer dataset containing customer demographics, service subscriptions, billing information, and churn status.

---

### Exploratory Data Analysis

**The following analyses were performed:**

- Distribution analysis of individual features using count plots and distribution plots.
- Comparison of churned and non-churned customers across categorical features.
- Boxplot analysis for numerical features against churn.
- Investigation of customer tenure, monthly charges, and total charges.
- Statistical hypothesis testing to evaluate feature associations with churn.

### Key Findings

- Higher churn was observed during the early stages of customer tenure.
- Customers with high monthly charges and relatively low total charges showed increased churn.
- Gender showed minimal impact on churn behavior.
- Most features demonstrated moderate to strong association with churn.

---

### Data Preprocessing

- Label Encoding applied to binary categorical features.
- One-Hot Encoding applied to multi-category features.
- Feature selection performed using statistical analysis.
- Total Charges was removed due to its dominance and limited additional contribution.

---

### Models Trained

The following machine learning models were evaluated:

1. Logistic Regression
2. Random Forest
3. XGBoost

---

### Model Optimization

**For each model:**

- Hyperparameter Tuning was performed.
- Threshold Tuning was performed to improve recall.
- Cross-validation was used during evaluation.

---

### Results

**Logistic Regression**

- Recall improved significantly after tuning.
- Reduced false negatives.
- Precision remained relatively low due to increased false positives.

**Random Forest**

- Achieved strong recall even before tuning.
- Further improved after hyperparameter and threshold tuning.
- Generated a larger number of false alarms.

**XGBoost**

- Showed limited improvement through hyperparameter tuning.
- Recall improved considerably after threshold tuning.
- Selected as the final model due to its overall performance.

---

**Conclusion**

- Customer churn prediction is a highly recall-sensitive problem because missing churn customers can directly impact business revenue.

- While none of the evaluated models achieved a perfect balance between recall and precision, XGBoost provided the most suitable trade-off
for identifying potential churn customers and was selected as the final model.

---

### *Note:*

- This was one of my earlier machine learning projects. While revisiting it later, I identified several areas where I could improve the exploratory data analysis, feature interpretation, and model evaluation process. I have kept the project as part of my learning journey and growth in machine learning.
