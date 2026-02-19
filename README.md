# Customer Satisfaction Prediction – Brazil Dataset

## Project Overview

This project analyzes demographic, socioeconomic, and technology awareness factors to predict customer satisfaction (Satisfied vs Unsatisfied) using machine learning models in KNIME.

The objective was to identify the key drivers of customer satisfaction and compare classification models to determine the most effective predictive approach.

---

## Business Problem

Which demographic and behavioral factors most strongly influence customer satisfaction in Brazil?

Can machine learning models accurately classify satisfied versus unsatisfied customers?

---

## Tools and Techniques

- KNIME Analytics Platform
- Decision Tree
- Random Forest
- Gradient Boosting
- Stratified Sampling
- Correlation Analysis
- Confusion Matrix Evaluation
- Precision, Recall, Specificity, F-score

---

## Data Description

The dataset includes:

- Demographic features (Age, Gender, Education, Residence)
- Income brackets
- Consumer preferences
- Technology awareness indicators
- Target variable: Customer satisfaction (Satisfied / Unsatisfied)

---

## Methodology

1. Data Cleaning
   - Verified no missing values
   - Checked for duplicate records

2. Data Filtering
   - Filtered dataset to include only Brazilian respondents

3. Exploratory Data Analysis
   - Correlation matrix analysis
   - Distribution analysis (age, income, gender, education, residence)

4. Data Partitioning
   - Applied stratified sampling
   - Tested multiple train-test splits (70:30, 62:38, 80:20)

5. Model Development
   - Decision Tree
   - Random Forest
   - Gradient Boosting

6. Model Evaluation
   - Precision
   - Sensitivity (Recall)
   - Specificity
   - F-score

---

## Model Performance Summary

| Model            | Best Split | F-Score (Satisfied) | F-Score (Unsatisfied)  |
|------------------|------------|---------------------|------------------------|
| Decision Tree    | 70:30      | 0.852               | 0.552                  |
| Random Forest    | 70:30      | 0.852               | 0.552                  |
| Gradient Boosting| 62:38      | 0.826               | 0.478                  |

Recommended Model: Random Forest (balanced predictive performance across both classes).

---

## Key Insights

- Technology awareness and trust-related features showed strong positive correlation with satisfaction.
- Random Forest provided the most stable and balanced performance.
- Decision Tree performed well when prioritizing satisfied customer classification.
- Gradient Boosting demonstrated strong sensitivity for satisfied customers but weaker unsatisfied detection.

---

## Repository Structure

## Repository Structure

```
brazil-customer-satisfaction-prediction
│
├── report/
│   └── Customer_Satisfaction_Prediction_Report.pdf
├── workflow/
│   └── knime_workflow.knwf
├── screenshots/
│   └── correlation_matrix.png
└── README.md
```


---

## Future Improvements

- Hyperparameter tuning
- Feature importance analysis
- Python implementation using scikit-learn
- Model explainability techniques (e.g., SHAP)

---

## Author

Shruthi Rajeshwari

