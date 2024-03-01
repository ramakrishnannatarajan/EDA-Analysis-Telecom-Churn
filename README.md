# Telecom Customer Churn Analysis

## Business Understanding and Overview

In the telecom industry, preventing customer churn is crucial for long-term success. This data analysis focuses on understanding customer attrition by conducting Exploratory Data Analysis (EDA) using Python. The goal is to uncover patterns and insights that guide informed decision-making.

### Target Variable
Initial findings show an overall churn rate of 26.58%, serving as our base target value for future comparisons.
![Overall Churn](Data/Images/Churn_Overall.png)
### Missing Data Analysis

#### Data Type Correction:
- "Total Charges" column data type corrected to float64 for accurate analysis.

#### Handling Null Values:
- 11 null records in "Total Charges" (0.15% of data) were dropped, resulting in 7032 records.
![Missing Values](Data/Images/Percentage_Missing_Values.png)
### Data Cleaning

#### Tenure Grouping for Visualization:
- "Tenure Months" grouped into six bins for improved visualization, creating a new column, "tenure_group."

#### Irrelevant Column Removal:
- "Customer ID" and "Tenure" dropped as irrelevant for focused analysis.

### Initial Findings of Univariate Analysis

- Converted categorical values to numerical using get_dummies.
- Explored correlations between numerical features and "Churn" column.
- Identified attributes associated with higher churn rates.
  
![Initial Findings](Data/Images/CvsAllData_Corr.png)

## Univariate Categorical Analysis Highlights

- Customers with attributes like month-to-month contracts (42.71%), no online security (41.78%), no tech support (41.65%) exhibit higher churn.
  
![Month to Month](Data/Images/CvsContract.png)

![Onine Security](Data/Images/CvsOnlineSecurity.png)

![Tech Support](Data/Images/CvsTechSupport.png)



## Next Steps Planned

1. **Detailed Bivariate Analysis:**
   - Conduct a detailed examination of how different factors relate to each other concerning customer churn through bivariate analysis.

2. **Insights Generation:**
   - Summarize key insights from the analysis to highlight crucial patterns and relationships.

3. **Machine Learning Prediction:**
   - Utilize insights to build a machine learning model predicting future churners.

4. **Data-Driven Decision Making:**
   - Integrate advanced analytics and machine learning for data-driven decisions, ensuring competitiveness in the telecom market.

**Stay tuned for further updates as we progress through the analysis!**
