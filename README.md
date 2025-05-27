# No-Churn-Telecom
Machine Learning Project 
## Problem Statement:
### 1) Identify Key Influencing Factors.
### 2) Understand behavior patterns and dissatisfaction reasons.
### 3) Create a predictive model for churn probability.
### 4) Predict Churn Customers with "CHURN-FLAG"
### 5) Assign YES (1) to likely churners and NO (0) to retained customers.

## Steps Involved:
### 1) Domain Study
### 2) Importing the data into jupyter from the SQL databse.
### 3) Importing Neccessary Libraries
i) numpy

ii) pandas

iii) matplotlib.pyplot

iv) seaborn

### 4) Basic Checks and Data Cleaning
i) Rename the columns as per the business case

ii) Checking the top and bottom entries for overview.

iii) checking the data types of the features.

iv) Checking for the null values.

v) Checking for duplicates.

### 5) EDA
i) In univariate analysis finding the descriptive statistics for the numerical features of the data.

ii) Ploting pie chart for the 'International Plan', 'VMail Plan', 'Churn' to check the percentage of yes or no.

iii) Ploting the countplot to check the customers across the various states.

iv) Ploting a chart to identify the average minutes at different times in a day (day time, evening time, night time).

v) Ploting chart to identify Charge per minute across arious times in a day ( average charge in day time, average charge in evening time, average charge in night time).

vi) Hypothesis testing (ANOVA).

vii) Multivariate analysis, Ploting heatmap of features to check multicollinearity.

### 6) Data Preprocessig and Feature Engineering
i) Converting the non numeric features into numeric using encoding.

ii) Data Balancing

iii) Standerdization

### 7) Model Implementation
i) Decision Tree

ii) Random Forests

iii) XGBoost

iv) KNN

v) SVM

vi) MLP Classifier

vii) Logistic Regression

### 8) Adding the CHURN-FLAG column.

### 9) Conclusion

### 10) Saving the best model

## Key Findings
### 1) Most of the customers who churn are more likely to do so around the 136-day mark. Therefore, focus on customers who are approaching that timeframe. The maximum number of customers are from the area code 415, so it's important to also focus on other areas.

### 2) Most of the customers do not have VMail plans, as it is not a priority. Therefore, the company can increase the cost of VMail plans and offer discounts on other plans, which may be beneficial for customer retention. It is the same for the international plan.

### 3) "The majority of the customers love to spend their evening time on calls, so providing offers for evening and night calls may be beneficial for customer retention."

### 4) "The main reason for churn may be that the average day call charges are higher than other time periods and also higher than the grand average, so it may be the reason for churn."

### 5) "Offering discounts to new customers and those who have been with the company for a long time may be beneficial for the company to retain the customers."

### 6) Model Saved
The XGBoost model demonstrates a high overall accuracy of 0.92 (92%) in predicting customer churn. The model is very effective at identifying non-churners (Class 0) with a precision of 0.93, a recall of 0.98, and an F1-score of 0.95. However, the performance for identifying churners (Class 1) is less robust, with a precision of 0.83, a recall of 0.61, and an F1-score of 0.71.
The lower recall for Class 1 indicates that the model misses a notable portion of actual churners, which may be attributed to the relatively lower number of observations for this class in the dataset. This imbalance can lead the model to prioritize the majority class (non-churners), resulting in reduced sensitivity for the minority class (churners).

