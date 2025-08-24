# Telco Customer Churn Prediction

This project explores customer churn prediction using machine learning techniques on a telco dataset. The goal is to identify customers who are likely to stop using the service, so proactive retention strategies can be developed.

---

## 📊 Project Overview
- **Dataset**: Telco customer churn data  
- **Objective**: Predict whether a customer will churn (`Yes`/`No`)  
- **Techniques Used**:
  - Data cleaning & preprocessing  
  - Handling class imbalance with **SMOTE**  
  - Random Forest classification  
  - Threshold tuning for precision/recall tradeoff  
  - Model evaluation with confusion matrices & metrics  

---

## ⚙️ Methodology
1. **Data Preprocessing**  
   - Handled missing values  
   - Converted categorical variables to factors  
   - Split data into training and test sets  

2. **Modeling**  
   - Trained a **Random Forest** classifier  
   - Compared results with and without class imbalance handling  
   - Adjusted classification threshold to optimize sensitivity vs. specificity  

3. **Evaluation Metrics**  
   - Accuracy  
   - Precision, Recall, F1-score  
   - Balanced Accuracy  
   - Kappa statistic  

---

## ✅ Results
- The tuned Random Forest improved detection of churned customers at the cost of some false positives.  
- Tradeoffs were analyzed using different thresholds.  
- Example confusion matrix performance (with threshold tuning):

| Metric              | Value   |
|---------------------|---------|
| Accuracy            | ~0.76   |
| Sensitivity (Recall)| ~0.78   |
| Specificity         | ~0.72   |
| Balanced Accuracy   | ~0.75   |

---

## 🛠️ Tools & Libraries
- **R** (base R + caret, randomForest,dplyr, recipes, nnet, ggplot2, recipes)  
- **R Markdown** for documentation and reporting  

---

 DATASET SOURCE
The Telco Customer Churn Dataset is publicly available on https://www.kaggle.com/blastchar/telco-customer-churn
