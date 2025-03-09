# Customer-Churn-Prediction-Using-Artificial-Neural-Network-ANN-
Customer Churn Prediction Using Artificial Neural Network (ANN)

Customer retention is a major concern for businesses, particularly in the banking and telecom sectors. Customer churn refers to customers who stop using a company's services. Identifying such customers early allows companies to take proactive measures to retain them.
In this project, we develop an Artificial Neural Network (ANN) classifier to predict customer churn based on customer demographics, financial data, and account activity. The model helps businesses reduce churn and improve customer relationship management (CRM).

Problem Statement

Objective:
To build an ANN-based predictive model that determines whether a customer will exit the bank (churn) based on their attributes.

Dataset Overview:
Source: Churn_Modelling.csv
Number of Customers: 10,000

Features:
Demographic: Geography, Gender, Age
Financial: Credit Score, Balance, Estimated Salary
Account-related: Number of Products, Active Member Status, Tenure

Target Variable:
Exited (Binary: 1 = Churn, 0 = Retained)

Business Impact:
Predict churn risk early.
Develop personalized retention strategies.
Improve customer engagement and profitability.

Methodology
1. Data Preprocessing
Removed unnecessary columns (RowNumber, CustomerId, Surname).
Encoded categorical features (Gender, Geography).
Normalized numerical features (MinMaxScaler applied).
Split dataset (80% train, 20% test).

3. ANN Model Architecture
Layer	Neurons	Activation
Input Layer	11	ReLU
Hidden 1	64	ReLU
Hidden 2	32	ReLU
Output	1	Sigmoid

5. Model Compilation & Training
Loss Function: Binary Crossentropy.
Optimizer: Adam.
Metrics: Accuracy.
Training: 50 epochs, batch size 32.

7. Evaluation Metrics
Accuracy: Measures how well the model classifies churn.
Precision & Recall: Useful for handling class imbalances.
Confusion Matrix: Evaluates False Positives and False Negatives.
