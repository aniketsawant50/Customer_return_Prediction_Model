# Customer_return_Prediction_Model
It is the customer return prediction model
# Customer Return Prediction (Machine Learning Project)

## Project Overview
This project focuses on predicting whether a customer will return to an e-commerce platform based on their behavior, engagement, and purchase history. The goal is to help businesses improve customer retention and make data-driven decisions.

---

## Problem Statement
The objective of this project is to build a machine learning model that predicts whether a customer will return (1) or not return (0) using historical customer data.

---

## Dataset
- Synthetic dataset with 5000 rows
- Contains customer behavioral and engagement features

### Features:
- Age  
- Gender  
- TotalPurchasesLast6Months  
- AvgOrderValue  
- BrowsingTime  
- DiscountUsage  
- CustomerSupportInteractions  
- DaysSinceLastPurchase  
- EmailClicksLastMonth  
- AppSessionsLastWeek  

### Target Variable:
- WillReturn  
  - 1 → Customer will return  
  - 0 → Customer will not return  

---

## Project Workflow

### 1. Data Preprocessing
- Handling missing values using median imputation  
- Encoding categorical variable (Gender)  
- Removing unnecessary columns (CustomerID)  

### 2. Exploratory Data Analysis (EDA)
- Univariate Analysis (distribution of features)  
- Bivariate Analysis (relationship with target variable)  
- Outlier detection using boxplots  

### 3. Feature Engineering
- Feature selection  
- Label encoding  
- Feature scaling using StandardScaler  

### 4. Model Building
The following classification models were used:
- Logistic Regression  
- Naive Bayes  
- Decision Tree  
- Random Forest  

### 5. Model Evaluation
Models were evaluated using:
- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix

### 6. Hyperparameter Tuning
- Used GridSearchCV
- 5-Fold Cross Validation
- Optimized parameters:
- n_estimators
- max_depth
- min_samples_split
- Evaluation metric: Recall

---

## Final Model
Random Forest performed the best among all models and was selected as the final model due to its high accuracy and robustness.
Random Forest Classifier (Tuned with GridSearchCV)
Reduced overfitting
Improved generalization
Optimized recall for better prediction of returning customers

---

## Key Insights
- Customers with higher purchases and spending are more likely to return  
- Engagement features like browsing time and app usage strongly influence return behavior  
- Recent activity (low days since last purchase) increases return probability  
- Low engagement and inactivity lead to customer drop-off  

---

## Business Impact
- Helps in identifying potential returning customers  
- Improves customer retention strategies  
- Enables targeted marketing campaigns  
- Increases overall business revenue  

---

## Tools and Technologies Used
- Python  
- Google Colab  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## How to Run
1. Open the Google Colab notebook  
2. Run all cells step by step  
3. Dataset will be generated or loaded  
4. Model will be trained and evaluated  

---

## Author
Aniket Sawant
