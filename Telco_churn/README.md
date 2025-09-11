# Telco Customer Churn Prediction

This project explores customer churn prediction using machine learning techniques on the Telco Customer Churn dataset. The goal is to identify customers likely to stop using the service, enabling proactive retention strategies.

## 📊 Project Overview
- **Dataset**: Telco Customer Churn data (publicly available on [Kaggle](https://www.kaggle.com/blastchar/telco-customer-churn))
- **Objective**: Predict whether a customer will churn (`Yes`/`No`)
- **Techniques Used**:
  - Data cleaning and preprocessing
  - Handling class imbalance with SMOTE
  - Random Forest, Logistic Regression, and Neural Network classification
  - Threshold tuning for precision-recall tradeoff (F1-based and pROC-based)
  - Model evaluation with confusion matrices, ROC curves, and metrics

## ⚙️ Methodology

### Data Preprocessing
- Handled missing values
- Converted categorical variables to factors and applied dummy encoding
- Split data into 80% training and 20% test sets
- Applied SMOTE to address class imbalance in training data

### Modeling
- Trained Random Forest, Logistic Regression, and Neural Network models
- Compared results with and without SMOTE
- Tuned classification thresholds to optimize sensitivity vs. specificity using:
  - Precision-Recall curve (F1 score maximization)
  - pROC curve (Youden’s J statistic)

### Evaluation Metrics
- Accuracy
- Precision, Recall, F1-score
- Balanced Accuracy
- Kappa statistic
- Area Under the ROC Curve (AUC)

## ✅ Results
- The tuned Random Forest (with SMOTE) improved detection of churned customers, though at the cost of some false positives.
- Threshold analysis revealed tradeoffs between sensitivity and specificity:
  - F1-based threshold captured more potential churners.
  - pROC-based threshold balanced sensitivity and specificity.
- Example performance metrics (with threshold tuning, approximate values):
  | Metric            | Value  |
  |-------------------|--------|
  | Accuracy          | ~0.76  |
  | Sensitivity (Recall) | ~0.78 |
  | Specificity       | ~0.72  |
  | Balanced Accuracy | ~0.75  |

## 🛠️ Tools & Libraries
- **R Packages**: `caret`, `randomForest`, `dplyr`, `recipes`, `nnet`, `ggplot2`, `pROC`, `themis`
- **Documentation**: R Markdown and Quarto for reporting
- **Visualization**: `ggplot2` for plots (saved in `plots/`)



 

