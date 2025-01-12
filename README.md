# **Customer Churn Prediction**

## **Overview**
This project builds a machine learning model to predict whether a customer will churn (stop using the bank's services). By identifying potential churners, the bank can take proactive steps to retain valuable customers.

---

## **Project Objectives**
- **Problem:** Determine customer churn with minimal false negatives due to higher associated costs.
- **Goal:** Build a model that improves recall (correctly identifying churners) to reduce potential losses.

---

## **Dataset**
- **Size:** 10,000 observations, 12 features.  
- **Key Features:**
  - **Demographics:** Geography, Gender, Age, Surname.
  - **Account Info:** CreditScore, Balance, NumOfProducts, IsActiveMember, Tenure.
  - **Target Variable:** Exited (Churn status: 1 = Yes, 0 = No).

---

## **Approach **

### **Situation**
The bank faces significant losses due to customer churn, with false negatives (missed churners) costing five times more than false positives.

### **Task**
Develop a machine learning model to predict churn, focusing on **recall** to minimize the number of missed churners.

### **Actions**
1. **Exploratory Data Analysis (EDA):**
   - Inspected data structure and distribution.
   - Checked for missing values and imbalances in the target variable.
   - Visualized relationships between features and churn.

2. **Data Preprocessing:**
   - Handled missing values, outliers, and categorical encoding (e.g., one-hot encoding).
   - Scaled numerical features for consistency.

3. **Model Development:**
   - Trained multiple models (Logistic Regression, KNN, Decision Tree, Random Forest, AdaBoost, Gradient Boost).
   - Evaluated models using **cross-validation**, prioritizing **recall** to reduce false negatives.

4. **Hyperparameter Tuning:**
   - Performed grid search for Gradient Boosting to optimize performance.

### **Results**
- Gradient Boosting emerged as the best model.
- **Model Improvement:** Recall score improved from **0.50 to 0.73** (a **46% improvement**).

---

## **Key Insights**
- False Negatives (missed churners) result in higher losses; focusing on **recall** ensures fewer at-risk customers are overlooked.
- Optimizing recall is crucial for scenarios where the cost of missed predictions outweighs false alarms.

---

## **Conclusion**
This project highlights how machine learning can identify at-risk customers, enabling the bank to take data-driven actions to retain clients and reduce churn-related losses.

Feel free to explore the code and analysis in this repository to understand the step-by-step process. 🚀

---
