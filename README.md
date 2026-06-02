# Customer-Churn-Prediction-ML
## Customer Churn Prediction using Machine Learning

## Project Overview

Customer churn is one of the most critical business challenges faced by telecommunication companies. Customer churn occurs when a customer stops using the company's services and switches to a competitor. Predicting customer churn enables businesses to take proactive measures to improve customer retention and reduce revenue loss.

This project develops a machine learning-based churn prediction system using the Telco Customer Churn dataset. The project includes data preprocessing, feature engineering, feature selection, model comparison, model training, and performance evaluation.

---

## Objectives

* Analyze customer behavior and churn patterns.
* Prepare and preprocess customer data.
* Identify important features influencing churn.
* Compare multiple machine learning algorithms.
* Select the best-performing model.
* Evaluate model performance using standard metrics.

---

## Dataset Information

The dataset contains customer information from a telecommunications company.

### Features Include:

* Gender
* Senior Citizen Status
* Partner
* Dependents
* Tenure
* Phone Service
* Internet Service
* Contract Type
* Monthly Charges
* Total Charges
* Payment Method

### Target Variable

Churn

* Yes = Customer left the service
* No = Customer retained the service

---

## Project Workflow

### Task 1: Data Preparation

* Loaded dataset using Pandas
* Checked missing values
* Converted TotalCharges to numerical format
* Removed invalid records
* Encoded categorical variables
* Prepared machine-learning-ready dataset

### Task 2: Train-Test Split

* Split dataset into:

  * 80% Training Data
  * 20% Testing Data
* Used stratified sampling

### Task 3: Feature Selection

* Correlation analysis
* Random Forest feature importance analysis
* Selected influential features

### Task 4: Model Selection

The following algorithms were evaluated:

* Logistic Regression
* Decision Tree
* Random Forest
* Gradient Boosting

### Model Comparison

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | 80.45%   |
| Gradient Boosting   | 79.53%   |
| Random Forest       | 78.54%   |
| Decision Tree       | 71.29%   |

Logistic Regression achieved the highest accuracy and was selected as the final model.

### Task 5: Model Training

* Trained Logistic Regression model
* Saved trained model for future use

### Task 6: Model Evaluation

Performance metrics were calculated using the testing dataset.

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | 80.45% |
| Precision | 64.86% |
| Recall    | 57.75% |
| F1 Score  | 61.10% |
| ROC-AUC   | 83.62% |

---

## Results

The Logistic Regression model demonstrated strong predictive capability with an ROC-AUC score of 0.836, indicating excellent separation between churn and non-churn customers.

The model successfully identified customer churn patterns using customer demographics, service usage, contract information, and billing attributes.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Joblib

---

## Repository Structure

Customer-Churn-Prediction-ML/

├── data/

├── notebooks/

├── models/

├── images/

├── report/

├── requirements.txt

└── README.md

---

## Future Improvements

* Hyperparameter tuning
* SMOTE for class balancing
* XGBoost implementation
* Deployment using Streamlit
* Real-time prediction dashboard

---

## Author

Abhishek

Machine Learning Internship Project
