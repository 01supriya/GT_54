# **GST 54 - GST HACKATHON**
## Introduction
The world of Data-Driven AI and ML solutions are being extensively used in solving many problems that exist in the world. While these used to be confined to the big tech companies, nowadays it is accessible to each and everyone. This has led to these concepts being used on wide-range of problems, ranging from Finance to Medical fields, improving the efficiency and driving these fields to the next level.

This made us wonder what if we use these concepts in building a predictive modelling for the Commercial Taxes (GST), which plays a significant role in contribution in terms of revenue to the country.

The Goods and Services Tax is an effort towards the simplification of the taxation process of goods and services by almost all countries. GST is expected to replace various indirect taxes such as sales tax and value-added tax, thereby unifying the very fragmented structure which seems more transparent and more compliant. GST also aims at streamlining tax administration while reducing cascading effects, ease of doing business being its third result. Hence, providing multi-tax slabs and with an appropriate input tax credit, GST will encourage businesses to maintain a proper record hence ensuring efficiency and an economy benefitting the consumer as well as the economy by minimizing tax evasions.

This is our submission towards the GST Hackathon in solving the problem statement using Data Science concepts available to offer the best possible solution.


## Problem Statement 
We have worked on a vast dataset of approximately 900,000 records, each containing around 21 attributes and target variables. This anonymized data is meticulously labeled and includes training, testing, and a non-validated subset for final evaluations by the GST Network (GSTN).

The problem statement given to us is as below:
Given a dataset D, which consists of:
Dtrain A matrix of dimension R(m×n) representing the training data.
Dtest A matrix of dimension R(m1×n) representing the test data.

We have also provided corresponding target variable Ytrain matrix dimension of R(m×1) and Ytest with matrix dimension of R(m1×1).

The objective is to construct a predictive model Fθ(X)→ Ypred that accurately estimates the target variable Y{i} for new, unseen inputs X{i}



## Project Implementation
1. **Exploratory Data Analysis (EDA)**  
   - Perform initial analysis to understand the datasets
   - Visualize key features and relationships.

2. **Data Cleansing**  
   - Handle missing or inconsistent data.
   - Remove duplicates and correct data types.
   - Normalize and prepare data for further analysis.

3. **Modeling and Feature Engineering**  
   - Select key features based on EDA.
   - Create new features if necessary (e.g., transformations, aggregations).
   - Split data into training and testing sets.
4. **Comparison of Metrics**  
   - Compare performance metrics across different models.
   - Evaluate accuracy, precision, recall, F1-score, etc.
   - Identify the best model based on defined business objectives.


## Exploratory Data Analysis
### Understanding the Training and Testing Data 
| Feature | Train Data | Validation Data |
|---|---|---|
| Rows | 779,140 | 261,712 |
| Duplicates | 0 | 0 |
| Features | 24 | 24 |
| Categorical | 9 | 9 |
| Numerical | 14 | 14 |
| Text | 1 | 1 |

From this, we can see that the Training data has 779140 Rows and 

