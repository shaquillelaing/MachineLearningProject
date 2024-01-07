# Marketing Campaign Optimization using Machine Learning

## Table of Contents

- [Project Overview](#project-overview)
- [Objective](#objective)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
- [Machine Learning Techniques Used](#machine-learning-techniques-used)
- [Results and Conclusion](#results-and-conclusion)

## Project Overview
This data analysis project aims to optimize a telephone-based direct marketing campaign for term deposits subsciptions for a fictional Canadian Bank: MapleTrust, using Machine Learning.
Intense competition with other financial institutions further emphasizes the need for effective marketing strategies. Current challenges exist in tailoring marketing approaches 
to individual clients, resulting in lower-than-desired term deposit purchases/subscriptions. MapleTrust wants to maximize returns on marketing investments, and capitalize on potential revenue from term deposit enrollments.
The aim is to develop a robust model, that can also be used to apply to furture marketing campaigns.

#### I am a post-graduate student enrolled in the Business Insights and Analytics Program at Humber College. This project was originally created as part of my group's project in the course Machine Learning 1 (BIA 5302), instructed by Dr. Salam Ismaeel. 
#### Contributors: Shaquille Laing, Tanishka Patil, Soumil Kapri, Riya Johnson and Grace Abunyie.

## Objective
The primary objective of this initiative is to develop a predictive model that accurately predicts whether a client will opt to purchase a term deposit (Yes/No), allowing the bank to better tailor its approach and enhance its marketing effectiveness.

## Data Source
[Download here](https://archive.ics.uci.edu/dataset/222/bank+marketing)

## About the Dataset
The dataset "bank.csv", represents telephone-based direct marketing interactions by MapleTrust Bank, aiming to predict whether clients will enroll in a term deposit. 

## Tools

- Jupyter Notebook (Python) [Download Here](https://jupyter.org/install)

### Data Cleaning and Preprocessing
1. In our analysis, the target variable originally labeled as 'y' was renamed to 'deposit' to better reflect its significance. This variable serves as a determinant, indicating whether a client will enroll in the term deposit.
2. To ensure faster processing of our algorithms, we removed unwanted features that were not relevant to our predictive model such as the ‘Day’ column.
3. We checked for any potential missing values in our dataset using the 'isnull()' function.
4. Categorical variables, such as 'job,' 'marital,' 'education,' and 'contact,' were encoded to change them to numeric variables.
5. Numerical features such as ‘balance’ and ‘duration’ were standardized to a common scale using StandardScaler() function.

### Machine Learning Techniques Used
1. Logistic Regression - Model used for predicting the probability of an event
2. K-Nearest Neighbours - Model that uses majority class or average of K-nearest data points in a feature space
3. Decision Tree - A tree like model that makes decisions based on a series of conditions
4. Random Forest - Multiple Decision Trees

### Results and Conclusion
For the initial analysis, all models yielded similar accuracy scores, making it challenging to pinpoint the best performer based on this metric alone. 
To address this imbalance and provide a more comprehensive evaluation, we turned our attention to the F1 score. The F1 score offers a balanced perspective by considering both precision and recall, especially beneficial in scenarios where class imbalances exist.
In the context of predicting client enrollment for deposits through telephone-based marketing at Maple Trust Bank, we adopted the F1 score as the primary metric for model evaluation. Random Forest emerged as the top performer, achieving a score of 40%.
