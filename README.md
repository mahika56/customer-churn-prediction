Customer Churn Prediction

Overview

Customer churn is a critical problem for businesses, as retaining existing customers is significantly more cost-effective than acquiring new ones.
This project focuses on building a **machine learning model to predict customer churn**, enabling proactive retention strategies.

Objective

To identify customers who are likely to churn based on their demographic and service usage data, and provide actionable business insights.

Dataset

* **Telco Customer Churn Dataset**
* Contains:

  * Customer demographics
  * Account information
  * Service usage details
  * Billing information

Tech Stack

* **Programming Language:** Python
* **Libraries:**

  * Pandas, NumPy
  * Matplotlib, Seaborn
  * Scikit-learn

Project Workflow

### 1️⃣ Data Preprocessing

* Handled missing values in `TotalCharges`
* Converted categorical variables using one-hot encoding
* Scaled features for Logistic Regression

### 2️⃣ Exploratory Data Analysis (EDA)

* Identified patterns in churn behavior
* Observed higher churn among:

  * Low tenure customers
  * High monthly charge users
  * Month-to-month contracts

### 3️⃣ Model Building

* Logistic Regression
* Random Forest Classifier

### 4️⃣ Model Evaluation

* Confusion Matrix
* Precision, Recall, F1-score
* ROC Curve & AUC

## Results

| Model               | Accuracy | Recall (Churn) | F1 Score |
| ------------------- | -------- | -------------- | -------- |
| Logistic Regression | 0.79     | 0.32           | 0.44     |
| Random Forest       | 0.80     | 0.45           | 0.54     |

**AUC Score: 0.85**

Key Insights

* Customers with **low tenure** are more likely to churn
* Higher **monthly charges** increase churn probability
* **Contract type** significantly impacts retention
* Customers using **electronic check payments** show higher churn
* **Fiber optic users** have higher churn rates

## Business Impact

* Helps companies **identify at-risk customers early**
* Enables **targeted retention strategies**
* Reduces **customer acquisition costs**

## Project Structure

Customer-Churn-Prediction/
│
├── data/
│   └── telco_churn.csv
│
├── customer_churn_prediction.ipynb
├── README.md
├── requirements.txt

## How to Run

```bash
# Clone repository
git clone https://github.com/your-username/customer-churn-prediction.git

# Install dependencies
pip install -r requirements.txt

# Run notebook
jupyter notebook

## Future Improvements

* Hyperparameter tuning for better recall
* Deployment using Streamlit
* Handling class imbalance using SMOTE
* Trying advanced models like XGBoost

## Author

**Mahika Jojee**

* Aspiring Data Scientist
* Passionate about pattern recognition and data-driven decision making

---

## ⭐ If you like this project

Give it a ⭐ on GitHub!
