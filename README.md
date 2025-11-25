# Salary Prediction Using Linear Regression

##  Project Overview
This project explores how years of experience influence salary using a simple machine learning model. The goal is to follow the CRISP-DM process to perform exploratory data analysis (EDA), clean the data, train a model, evaluate it, and communicate insights through a blog post.

##  Dataset
The dataset contains 10 rows with the following columns:
- `years_experience` — numeric
- `degree` — categorical
- `bootcamp` — categorical
- `salary` — numeric (target variable)

##  Tools & Libraries
- Python  
- pandas  
- numpy  
- scikit-learn  
- matplotlib  
- seaborn  

## CRISP-DM Summary
### **1. Business Understanding**
Predict salary using experience-based data.

### **2. Data Understanding**
EDA showed a strong positive linear relationship between years of experience and salary.

### **3. Data Preparation**
Dataset contained no missing values. Categorical features were not used in the model due to small sample size.

### **4. Modeling**
A linear regression model was trained using:

### **5. Evaluation**
- **R² Score:** 0.9880  
- **MSE:** 6,864,443.65  
Model shows excellent predictive performance.

### **6. Deployment / Communication**
A clear blog post summarizing findings was published.

##  Prediction Example
For a person with **4.5 years** of experience:

