# Predict employee churn using random forest 

## Overveiw
The goal of this project is to identify features that determine or influence an employee to leave the company. This project used data from [Kaggle](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction?select=HR_comma_sep.csv). The random forest model performed with an accuracy of 0.98, precision of 0.98, recall of 0.92 and f1  of 0.95 in predicting which employee will leave the company. Based on the model, satifsfaction level, number of projects, tenure, averange monthly hours, and last evaluation were the most important determinants of employee's departure.

## Bussiness understanding
According to [Hubstaff](https://hubstaff.com/blog/working-days-in-a-month/#:~:text=has%2021%20days.-,How%20many%20average%20working%20days%20are%20in%20a%20month%3F,to%20176%20hours%20every%20month.), the average normal monthly working hours is between 160 and 176. It is important to learn how working hours could influence employee's departure.

## Understanding data
Our data has **14999 observations and **10 columns; out of these observations **3008 were duplicates which were later dropped. The data includes features like employee's tenure, average monthly hours, number of projects etc. The data has 84% of stayed employees and 16% of departed employees. Salary colum was an ordinal categorical variable and was encoded into a new variable called salary_code.

## Model evaluation
A random forest model comprising 100 decision trees was used to determine feature importance. The below plot show the top five important features. 
[Important features](.project\viz\important_features.png)
The overall model performed with 86% accuracy and 72% precision.
