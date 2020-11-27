# [employee-attrition-predictor](https://github.com/parthshah28/Human_Resources_Department)
A model that could predict which employees are more likely to quit.

## WEB APP - [Click Here](https://employee-attrition-predictor.herokuapp.com/home)

## **Understanding The Project**

### **The Dataset**

[Dataset](https://www.kaggle.com/pavansubhasht/ibm-hr-analytics-attrition-dataset)


## **Overview**
* Dataset has **1470 rows** and **35 columns**.
* We have to predict which employees are more likely to quit.
* I have replaced the **'Attritition' and 'overtime'** column with integers


## Feature Engineering

### A. Prepare the data
* I checked for missing data then I dropped **'EmployeeCount' , 'Standardhours' and 'Over18'** since they do not change from one employee to the other and I dropped **'EmployeeNumber'** as well.

* **Total = 1470**
* **Number of employees who left the company = 237**
* **Percentage of employees who left the company = 16.122448979591837 %**
* **Number of employees who did not leave the company (stayed) = 1233**
* **Percentage of employees who did not leave the company (stayed) = 83.87755102040816 %**

<table><tr><td><img src='https://github.com/parthshah28/Human_Resources_Department/blob/main/images/1.png'></td><td><img src='https://github.com/parthshah28/Human_Resources_Department/blob/main/images/2.png'></td><td><img src='https://github.com/parthshah28/Human_Resources_Department/blob/main/images/3.png'></td></tr></table>


### B. Data Cleaning 
* I converted categorical variables **'BusinessTravel', 'Department', 'EducationField', 'Gender', 'JobRole', 'MaritalStatus'** into numeric variables using **OneHotEncoder.**

### C. Feature Scaling
For scaling, **MinMaxScaler** has been applied.

**to understand it in more detail go to [Human_Resources_Department](https://github.com/parthshah28/Human_Resources_Department/blob/main/Human_Resources_Department.ipynb)**

***
### **Applied Algorithms & Their Accuracy**
***
| Algorithm | Accuracy |
| ---    | ---    |
| Random Forest | 90.28% |
| Logistic Regression |  89.94% |



