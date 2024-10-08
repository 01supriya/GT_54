**GST 54 - GST HACKATHON**
===================================================

## Introduction


The world of Data-Driven AI and ML solutions are being extensively used in solving many problems that exist in the world. While these used to be confined to the big tech companies, nowadays it is accessible to each and everyone. This has led to these concepts being used on wide-range of problems, ranging from Finance to Medical fields, improving the efficiency and driving these fields to the next level.

This made us wonder what if we use these concepts in building a predictive modelling for the Commercial Taxes (GST), which plays a significant role in contribution in terms of revenue to the country.

The Goods and Services Tax is an effort towards the simplification of the taxation process of goods and services by almost all countries. GST is expected to replace various indirect taxes such as sales tax and value-added tax, thereby unifying the very fragmented structure which seems more transparent and more compliant. GST also aims at streamlining tax administration while reducing cascading effects, ease of doing business being its third result. Hence, providing multi-tax slabs and with an appropriate input tax credit, GST will encourage businesses to maintain a proper record hence ensuring efficiency and an economy benefitting the consumer as well as the economy by minimizing tax evasions.

This is our submission towards the GST Hackathon in solving the problem statement using Data Science concepts available to offer the best possible solution.


## Problem Statement 

We have worked on a vast dataset of approximately 900,000 records, each containing around 21 attributes and target variables. This anonymized data is meticulously labeled and includes training, testing, and a non-validated subset for final evaluations by the GST Network (GSTN).

**Problem Statement:**

Given a dataset **D** consisting of:

* **Dtrain:** A matrix of dimension $R(m \times n)$ representing the training data.
* **Dtest:** A matrix of dimension $R(m1 \times n)$ representing the test data.

And corresponding target variables:

* **Ytrain:** A matrix of dimension $R(m \times 1)$.
* **Ytest:** A matrix of dimension $R(m1 \times 1)$.

The objective is to construct a predictive model **Fθ(X) → Ypred** that accurately estimates the target variable **Y{i}** for new, unseen inputs **X{i}**.

## Project Implementation
1. **Exploratory Data Analysis (EDA)**  
   - Preliminary Analysis of the Datasets
   - Univartiate Analysis
   - Bivariate Analysis
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
### <ins>Understanding the Training and Testing Data</ins>
#### Basic Analysis
| Feature | Train Data | Validation Data |
|---|---|---|
| Rows | 779,140 | 261,712 |
| Columns | 24 | 24 |
| Duplicate Rows | 0 | 0 |
| Categorical | 9 | 9 |
| Numerical | 14 | 14 |
| Text | 1 | 1 |



##### <ins>Observation</ins>:

 - The **Train Data** consists of ***779140** Observations* and ***24** Features* and **Test Data** consists of ***779140** Observations* and ***24** Features*
- Both of the datasets **do not**  have any duplicateobservations.
- Both the datasets have **9 Categorical Features**, **14 Numerical Features**, and **1 Text Feature**.

## Univariate and Bi-Variate Analysis
*The Univariate Analysis was carried out on both train and validation data to see the difference in the features in terms of their observations. While  the Bivariate Analysis would be done primarily on the Train Data where some important relations were seen.*

<img src="https://github.com/user-attachments/assets/05538e9b-7b77-444a-816e-625ef98152af" width="300" alt="image">
<br>

## TEXT
### ID Column
<img width="450" alt="image" src="https://github.com/user-attachments/assets/5aceac39-c292-4cee-8b28-ae9e2b6467f7">

## CATEGORICAL
### Target Column
<img width="215" alt="image" src="https://github.com/user-attachments/assets/e0f1d9f1-79e1-46ba-85c2-02517b91d8c6">

### Column10
<img width="215" alt="image" src="https://github.com/user-attachments/assets/a500754a-8ef4-4033-8504-051b2322f10c">

### Column11
<img width="212" alt="image" src="https://github.com/user-attachments/assets/56e40166-5605-4d73-b7b6-770525fa2a73">

### Column12
<img width="212" alt="image" src="https://github.com/user-attachments/assets/de7c866b-ff98-4923-aa47-9833ef742530">

### Column13
<img width="212" alt="image" src="https://github.com/user-attachments/assets/17541fda-f974-4249-bbf4-f63bda439efb">

### Column16
<img width="218" alt="image" src="https://github.com/user-attachments/assets/a4c4c225-10ca-45b8-a021-37b3321653b6">

### Column19
<img width="214" alt="image" src="https://github.com/user-attachments/assets/1cee06a5-7ba4-4530-928c-15bde6e9175a">

### Column20
<img width="211" alt="image" src="https://github.com/user-attachments/assets/1e35307b-5840-4579-bdda-6f3000a49b90">

### Column21
<img width="215" alt="image" src="https://github.com/user-attachments/assets/a10755bc-2995-401e-a29c-57203353b70b">

## NUMERICAL
### Column0
<img width="467" alt="image" src="https://github.com/user-attachments/assets/31bc49c3-273d-4ab6-843f-2bce8ccbfd51">
<br>
<img width="319" alt="image" src="https://github.com/user-attachments/assets/4a8f1587-7b63-495d-b897-1dd70863f6a0">

### Column1
<img width="355" alt="image" src="https://github.com/user-attachments/assets/b6d49441-3e29-455f-a1c5-5359d7c5b6d2">
<br>
<img width="320" alt="image" src="https://github.com/user-attachments/assets/d3646db1-858e-4054-bb15-08e00fb0cae8">

### Column2
<img width="353" alt="image" src="https://github.com/user-attachments/assets/c284e64b-71df-4886-943b-c373d37dc3cf">
<br>
<img width="317" alt="image" src="https://github.com/user-attachments/assets/6aae92f3-4aaf-4bb4-8cfc-1df09a560581">

### Column3
<img width="359" alt="image" src="https://github.com/user-attachments/assets/26d05726-da72-49ad-a359-f419e3eb0911">
<br>
<img width="316" alt="image" src="https://github.com/user-attachments/assets/d29bf7ab-73b1-45cc-abaa-4282e87fe913">

### Column4
<img width="352" alt="image" src="https://github.com/user-attachments/assets/fff51a5d-457a-4f41-a946-e57463147cf0">
<br>
<img width="319" alt="image" src="https://github.com/user-attachments/assets/7583d6ea-3fd0-4f46-aaa2-7ab57b6049b8">

### Column5
<img width="356" alt="image" src="https://github.com/user-attachments/assets/1a416228-4a55-4b96-a217-136b22e549ff">
<br>
<img width="324" alt="image" src="https://github.com/user-attachments/assets/f5587784-a262-478c-bfda-ebebc09bae38">

### Column6
<img width="347" alt="image" src="https://github.com/user-attachments/assets/c05bb705-bd7b-4c9e-987f-d38fb0a47f36">
<br>
<img width="326" alt="image" src="https://github.com/user-attachments/assets/067bfd46-fccf-4d36-970e-eb3b588dec05">

### Column7
<img width="353" alt="image" src="https://github.com/user-attachments/assets/36d268a9-89cb-43b5-bd57-abdda876b0c5">
<br>
<img width="323" alt="image" src="https://github.com/user-attachments/assets/cc3bfd0b-3b6f-469b-b6aa-499c9af4de32">

### Column8
<img width="350" alt="image" src="https://github.com/user-attachments/assets/260409a7-be11-428d-bb13-b2c8d3d89ed8">
<br>
<img width="323" alt="image" src="https://github.com/user-attachments/assets/fc84d11a-4f18-4afa-9d7c-c6fd2544596f">

### Column9
<img width="352" alt="image" src="https://github.com/user-attachments/assets/0c9cb44a-e325-4a51-8be7-e4e81fc6b66b">
<br>
<img width="316" alt="image" src="https://github.com/user-attachments/assets/976c86eb-24be-4710-8c12-3649e0a39eda">

### Column14
<img width="348" alt="image" src="https://github.com/user-attachments/assets/503e245f-8128-4e5c-810d-4f99bd0b80a2">
<br>
<img width="320" alt="image" src="https://github.com/user-attachments/assets/9813f318-c82f-4f06-95da-e8c4891b0d73">

### Column15
<img width="352" alt="image" src="https://github.com/user-attachments/assets/3862e361-c876-4a5f-84c5-a8a741f26050">
<br>
<img width="323" alt="image" src="https://github.com/user-attachments/assets/21dd4446-92c4-44ea-b353-2749c1fc2929">

### Column17
<img width="358" alt="image" src="https://github.com/user-attachments/assets/4cd0c4da-ea0b-44b7-b1f3-4fc749762da6">
<br>
<img width="329" alt="image" src="https://github.com/user-attachments/assets/4cd7f62b-a1c5-4d3f-b667-dd79564cf29c">

### Column18
<img width="353" alt="image" src="https://github.com/user-attachments/assets/6454426e-9acf-463b-bdaf-ef3755c506f0">
<br>
<img width="321" alt="image" src="https://github.com/user-attachments/assets/4978daa1-0c6d-4509-a0c5-56677698d7af">

##### <ins>Observations</ins>:
 - The **ID**column has no missing values meaning all the observations are unique.
 - All the **Categorical** variables have only **One** missing value each
 - The **Target** variable is *highly imbalanced* with two classes split at **91%** and **9%**. This is the similar case for other categorical variables such as       *Column16,Column19,Column20,Column21.*
 - The variablese such as *Column3, Column4, have around **16%** of observations as missing values, with *Column5* having around **21%**. It has to be noted that the ***Column9*** has around ***93%*** of the observations as missing values.

## Bi-Variate Analysis
### Correlation between Variables
The **Correlation Coefficient** helps us understand the strength of the linear relationship between two variables. The value ranges from *-1 to 1*.
   - If the **correlation coefficient is less than zero**, it means the variables have an *inverse relationship* — when one goes up, the other tends to go down.
   - If the **correlation coefficient is greater than zero**, it indicates a *direct relationship* — both variables tend to move in the same direction.
   - If the **correlation coefficient is zero**, it suggests that the variables are *not related* — there’s no clear pattern in how they move together.

   --We have used the **Pearson's Correlation Coefficient** to calculate the Correlation which is as below:
The correlation coefficient \( r \) is given by:

$$
r = \frac{\sum{(x - \bar{x})(y - \bar{y})}}{\sqrt{\sum{(x - \bar{x})^2} \sum{(y - \bar{y})^2}}}
$$

where:
* $\bar{x}$ is the average of $n$ values of $x$
* $\bar{y}$ is the average of $n$ values of $y$

In the ideal situation, the  variables should have *higher correlation* with the target variable but must have *low correlation* within themselves. Hence we plotted a Correlation Matrix for the *train* to understand the *Correlation between each of the variables.

#### Correlation Matrix for Train Data
<img width="600" alt="image" src="https://github.com/user-attachments/assets/9b6b13ae-40f8-454d-857f-ab9dd8179cb3">

##### Visualize key features and relationships.
 - *From the above *Correlation Matrix*, we can see that Column3 & column4 have *High* Correlation wtihin themselves. So we plotted a *Scatter Graph* to understand the correlation. *

 <img width="359" alt="image" src="https://github.com/user-attachments/assets/716ca45a-e4d1-4a2b-ab40-5d3ddc66e660">










