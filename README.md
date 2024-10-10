
# Project Overview
This project aims to develop a machine learning model to predict customer churn for a telecom company. The goal is to identify potential churn risks and provide insights to improve customer retention strategies.

## Project Highlights🚀
- Conducted exploratory data analysis to uncover insights and patterns within the dataset. 
- Built predictive models using machine learning algorithms like Random Forest Classifier.
- Developed a Power BI dashboard for interactive visualization of key findings.

## Contains
- Library Imports
- File Operations
- Exploratory Data Analysis (EDA)
- Data Cleaning
- Feature Engineering
- Model Building
- Model Comparison

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Seaborn
- Matplotlib
- Flask
- Power BI

## Data Preprocessing
- Conducted data cleaning and transformation to enhance data quality.
- Handled missing values - TotalCharges are replaced with NaN and rows with missing values are dropped.
- Feature Engineering - Converting categorical features to numerical features using **Label encoding** , Target variable Churn is extracted.

## Exploratory Data Ananlysis (EDA)
- Questions to address:

What is the proportion of customers who have churned versus those who have not churned?
![](https://github.com/user-attachments/assets/7237519f-e4ce-496e-8ce4-be4d3368936f)

How does the monthly charges vary between customers who have churned and those who have not?
![](https://github.com/user-attachments/assets/b2dd59bc-12d6-4ba6-ba63-fbaa528ef130)

How does the proportion of churn vary across different contract types (month-to-month, one year, two-year)?
![](https://github.com/user-attachments/assets/8191ca47-d518-4e21-b081-537ccb109c03)

How does the presence or absence of internet service affect customer churn rates?
![](https://github.com/user-attachments/assets/dbffba34-4a63-4bec-9fc0-6651b521c787)

5. How does the type of internet service (DSL, Fiber Optic, None) influence monthly charges and customer churn?
![](https://github.com/user-attachments/assets/58127f14-2769-4c17-89ad-b19be2de7a3a)


## Statistical Tests 
- feature selection techniques such as ANOVA test( F1-score) and chi-square test which improved model performance.
- Chi Square Test (categorical_features)
![](https://github.com/user-attachments/assets/f1526a5d-6210-4fee-b58a-c04ca3ef7a8d)
- Contract has the highest score because it strongly influences customer churn. Short-term contracts offer flexibility, leading to higher churn,while long-term contracts create retention, - making it a key predictor of customer behavior.

- Anova Testing (Numerical features) or F-score
![](https://github.com/user-attachments/assets/b550f0cc-084f-436a-82c1-8ea4432ef853)
- "Tenure" has the highest ANOVA score, indicating its strong influence on predicting customer churn.

## Correlation 
![](https://github.com/user-attachments/assets/e6b6c0ab-1134-4ec8-98e5-166b1e7c947f)


## Feature importance using Random Forest
![](https://github.com/user-attachments/assets/5f017d25-d6ec-477f-8ca8-b95fe33c50ed)
- As shown in above graph total charges , monthly charges ,tenure and contract are significant features by using Random Forest feature_importance

## Normalization (Standardization)
- Feature scaling for numerical_features - ['tenure', 'MonthlyCharges', 'TotalCharges']

## Model Development
- Built a customer churn prediction model using various algorithms, including Logistic Regression, Random Forest, and Support Vector Machine (SVM).

## Model Comparison
| Accuracy Score | Model Name    |
|----------------|---------------|
| 0.80           | SVM           |
| 0.79           | LR            |
| 0.77           | KNN           |
| 0.77           | XGB           |
| 0.77           | RANDOM_F      |


## Results
- Achieved an accuracy of **80%** with the Logistic Regression model, with additional performance metrics indicating:
  - Precision: 0.62
  - Recall: 0.43
  - F1-Score: 0.50
