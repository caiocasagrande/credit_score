# Credit Score Project
## Overview
Enhancing Profitability with Prudent Risk Management for a Conservative Bank.

## Business Description
This project focuses on developing an in-house risk model for a conservative bank to facilitate informed lending decisions. The goal is to optimize profitability while maintaining a cautious approach and minimizing risk exposure.

## Understanding Credit Scores
A credit score is a crucial tool used by banks to assess the creditworthiness of borrowers. It involves analyzing various factors such as annual income, home ownership status, loan amount, and interest rate to make informed lending decisions.

## Key Factors Impacting Credit Scores
- Borrower's annual income in relation to loan amount
- Home ownership status
- Loan amount
- Interest rate

## Business Problem
**Challenge: Developing a Risk Model**

The primary challenge is to create a robust risk model aligning with the bank's philosophy of minimizing risk exposure. Key financial parameters considered include a $100 profit from each good customer and a $500 expected loss from each bad customer.

## Exploratory Data Analysis
Before diving into the machine learning models, I performed a exploratory data analysis (EDA) to understand the dataset.

### Data Cleaning
**Dropping Duplicates:** I started by removing any duplicate records in the dataset to ensure data integrity.

**Exploring Unusual Values:** A careful examination of the data was conducted to identify and address any unusual or unexpected values.

### EDA
Target Variable Distribution
- Examined how the target variable (Loan Status) is distributed throughout the dataset.

Numerical Variable Distribution
- Analyzed the distribution of numerical variables to identify patterns and potential outliers.

Impact of Age on Loan Status
- Explored whether the age of the person might have an impact on loan status.

Impact of Income on Loan Status
- Investigated the relationship between income and loan status.

Loan Intent Analysis
- Explored the main reasons for loan intent to understand borrower motivations.

Home Ownership and Loan Status
- Analyzed the distribution of home ownership with respect to loan status.

Loan Status by Loan Grade
- Investigated how loan status varies across different loan grades.

Relationship between Loan Interest Rate and Loan Amount
- Explored the correlation between loan interest rate and loan amount.

Loan Interest Rate Distribution by Loan Status
- Analyzed how loan interest rate is distributed for different loan statuses.

Outliers Analysis
- Conducted an analysis to identify and handle outliers in the dataset.

## Analysis Conclusions
- Borrower age has limited relevance in determining loan status.
- Individual income does not significantly influence loan status.
- Loan-to-income ratio is a crucial factor, with higher ratios indicating a higher likelihood of default.
- Loan intent influences loan status, with education, medical expenses, and ventures being common purposes.

## Feature Engineering and Data Preparation
Encoding for Categorical Variables
- Applied appropriate encoding techniques to handle categorical variables in the dataset.

Correlation Heatmap
- Utilized a correlation heatmap to visualize relationships between features.

KNN Imputation
- Employed K-nearest neighbors (KNN) imputation to address missing values.

Transformations
- Applied standard scaling and robust scaling transformations to ensure uniformity and robustness in the data.

## Machine Learning Models

**Model Selection**

The CatBoostClassifier excelled in the following areas:
- **Accuracy:** It demonstrated the highest accuracy among the tested models.
- **Confusion Matrix:** The confusion matrix revealed robust performance in correctly classifying both default and non-default cases.
- **Classification Report:** Precise evaluation metrics, such as precision, recall, and F1 score, further confirmed the model's effectiveness.

The CatBoostClassifier model provides the best metrics compared to other models (LGBMClassifier and RandomForestClassifier).

## Results and Strategies
- The project recommends a conservative loan approval strategy based on top-performing customer deciles.
- Strategic decision-making involves balancing customer base growth and effective risk management.
- Profitability is maximized in the first five deciles, with a 93.7% avoidance of high-risk customers.
- The eighth decile represents the peak of profitability but comes with higher exposure to higher-risk customers.

## Conclusion
This Credit Score Project aims to improve profitability for a conservative bank through informed decision-making. The recommended strategy involves selecting top-performing customer deciles to optimize profitability while adhering to a cautious approach.
