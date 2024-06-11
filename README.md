# Credit Card Fraud Detection Analysis

## Overview

This report details the methodology and insights derived from analyzing a dataset of credit card transactions to identify fraudulent activities. The primary objective was to leverage machine learning techniques to classify transactions accurately as fraudulent or non-fraudulent. This endeavor involved comprehensive data exploration, intelligent feature engineering, and strategic model selection and tuning.

## Dataset

The dataset comprises:
- 555,719 training observations
- 69,465 testing observations

Each observation represents an individual credit card transaction with various attributes. Initial exploration revealed a mix of numerical and categorical features, including transaction amount, date and time, merchant details, and customer demographics.

## Impact on Career

Working on this project has significantly enhanced my skills in data science and software engineering. It has deepened my understanding of machine learning, particularly in handling real-world challenges such as imbalanced datasets and the need for robust feature engineering. These insights and experiences are invaluable as I advance in my career, providing a strong foundation for tackling complex problems in various domains.

## Data Exploration

### Key Steps:
- Assessing missing values to ensure data quality for modeling.
- Visualizing the distribution of the target variable to highlight an imbalanced class distribution favoring non-fraudulent transactions.
- Plotting numerical features to identify potential outliers and trends.

### Insights:
- Fraudulent transactions often have amounts below $10,000.
- Fraudulent activities tend to peak during certain times of the day (12-11pm) and on specific days of the week (Monday, Tuesday, Sunday).
- Certain merchant categories and demographic factors (age groups, jobs) are more associated with fraud.

## Feature Engineering

### Techniques Used:
- Created features to capture extreme values in transaction amounts.
- Incorporated temporal features like `hour_of_day` and `day_of_week` to leverage patterns in predicting fraud.
- Highlighted transactions in high-risk merchant categories.
- Included demographic information to provide additional context for the model.

### Findings:
- People aged 40-70 are more likely to fall victim to fraud.
- Some states or companies may have insufficient resources to fight fraud-related transactions effectively.

## Model Selection and Performance

### Models Evaluated:
1. **K-Nearest Neighbors (KNN)**
   - Initial F1 Score: 0.926
   - Optimized F1 Score: 0.668
2. **Ensemble Classifier**
   - F1 Score: 0.369
3. **XGBoost**
   - F1 Score: 0.833

### Key Points:
- XGBoost outperformed others due to its ability to handle imbalanced datasets and model complex relationships.
- KNN's high initial score highlighted its effectiveness in capturing local fraud patterns but was computationally intensive.
- The ensemble method underperformed due to the dilution of strong signals when averaged with other models.

## Challenges and Solutions

### Imbalanced Data:
- Imbalanced datasets led to high accuracy but poor practical utility in detecting fraud.
- Focus on F1 score, precision, and recall rather than accuracy.
- Strategies like adjusting classification thresholds and using ensemble classifiers were employed to improve performance.

### Continuous Iteration:
- The necessity of continuous iteration and experimentation in model development was underscored to find the optimal balance between identifying fraudulent transactions accurately and maintaining a manageable false positive rate.

## Conclusion

This exploration into credit card fraud detection underscored the importance of comprehensive data analysis, innovative feature engineering, and meticulous model selection. The KNN and XGBoost models stood out for their performance, attributed to their ability to handle imbalanced data and leverage engineered features effectively. The insights gained not only facilitated the development of a high-performing classifier but also shed light on behavioral patterns associated with fraudulent transactions.

## Future Directions

Continued improvement of fraud detection systems, leveraging advancements in machine learning, and refining feature engineering techniques to adapt to evolving fraud patterns will be critical. This project serves as a testament to the impact of data-driven approaches in enhancing security and reliability in financial transactions.

---

Mariano Eliseo Majano Amaya
