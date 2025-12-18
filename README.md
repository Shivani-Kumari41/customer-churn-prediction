# Customer Churn Prediction using Machine Learning

## Overview
This project builds an end-to-end machine learning pipeline to predict customer churn in the telecom domain. The goal is to identify customers at risk of leaving and extract insights that can support retention strategies.

## Dataset
Telecom customer dataset containing demographics, service usage, billing information, satisfaction scores, and churn indicators.

**Target Variable**
- `Churn Label`: Yes / No (converted to 1 / 0)

## Tools & Libraries
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

## Approach
1. **Data Loading & Cleaning**
   - Loaded the dataset and standardized column names.
   - Converted the churn label to a binary target.

2. **Missing Value Handling**
   - Numeric features filled using median.
   - Categorical features filled using mode.

3. **Feature Engineering**
   - Dropped identifier columns (Customer ID).
   - One-hot encoded categorical variables.

4. **Train-Test Split**
   - Used stratified sampling to preserve churn class distribution.

5. **Model Training**
   - Trained a Logistic Regression model.

6. **Model Evaluation**
   - Evaluated using accuracy, confusion matrix, and classification report.

## Results
- **Accuracy:** ~91%
- **Recall (Churn class):** ~0.81

The model performs well in identifying churn-risk customers while maintaining strong overall accuracy.

## Key Business Insights
- Customers with month-to-month contracts show higher churn rates.
- Higher monthly charges are associated with increased churn.
- Long-tenure customers are less likely to churn.

## Conclusion
This project demonstrates a complete churn prediction workflow, from data preprocessing to model evaluation. It highlights how machine learning can be used to support customer retention decisions through data-driven insights.

## Notes
This is a learning-focused academic project. Future improvements could include feature selection, handling high-cardinality features, and trying alternative models.
