# Salary Prediction Using Machine Learning  
### A CRISP–DM Guided Data Science Project

This project analyzes a small salary dataset to understand how **years of experience influence salary**.  
Using the CRISP–DM framework, we explore the data, prepare it for modeling, train a linear regression model, evaluate performance, and create a real-world prediction scenario.

---

# Business Questions

This project is guided by five key questions:

1. **How does years of experience relate to salary?**  
2. **Can we build a machine learning model that predicts salary based on experience?**  
3. **How accurate is the model in explaining salary variation?**  
4. **What salary can we expect for a new candidate with a specific level of experience (e.g., 4.5 years)?**  
5. **Why were the categorical variables (`degree`, `bootcamp`) excluded from the model?**

---

# CRISP–DM Framework Summary

### **1. Business Understanding**
The goal is to help individuals estimate salary expectations based on professional experience.  
A simple, interpretable model is preferred for clarity and communication.

### **2. Data Understanding**
The dataset contains 10 samples with four features:
- `years_experience` — numeric  
- `degree` — categorical  
- `bootcamp` — categorical  
- `salary` — numeric (target)

Exploratory analysis included:
- Dataset summary  
- Distribution plots  
- Scatter plot of experience vs salary  

### **3. Data Preparation**
- Verified no missing values  
- Categorical variables were intentionally **excluded**  
  - Very small dataset (10 rows)  
  - Encoding categories would add unnecessary complexity  
  - Could cause overfitting  
- Selected `years_experience` as the predictor  

### **4. Modeling**
A **Linear Regression** model was trained using an 80/20 train-test split.

### **5. Evaluation**
Model performance metrics:

- **R² Score:** 0.988  
- **MSE:** 6,864,443.65  

The model explains **98.8% of the variation** in salary — excellent for this dataset.

### **6. Deployment / Scenario Prediction**
To demonstrate real-world use, we predicted the salary for:

> A candidate with **4.5 years of experience**

**Predicted Salary:**  
### **$74,331 (approx.)**

---

# Repository Structure

course2/
│── salary_prediction_project.ipynb # Jupyter notebook (CRISP–DM, EDA, modeling, scenario)
│── salary_dataset.csv # Dataset used in the project
│── README.md # Project overview and documentation
# Tools & Libraries Used

This project uses standard Python data science tools:

- **pandas**  
- **numpy**  
- **matplotlib**  
- **seaborn**  
- **scikit-learn**  
