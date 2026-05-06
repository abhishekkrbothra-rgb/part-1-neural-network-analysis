# part-1-neural-network-analysis- customer churn
Task 1: Dataset Understanding

Dataset Name: customer_churn_nn.csv

Total Rows: 2,000  

Total Columns: 17  

The Goal: Predict if a customer will leave (Churn = 1) or stay (Churn = 0).

Data Observation: The data is "imbalanced." Only 1.55% of customers in this list have churned. This means the AI needs to be very precise to find those few people.

Missing Values: None. The data is clean.  

Features: We have 4 categorical features (like Region) and several numerical features (like Monthly Charges).

# Task 2: Data Preprocessing
Feature Selection: Removed customer_id as it provides no predictive value.

Encoding: Converted categorical variables (region, plan_type, etc.) into numerical format using Label Encoding.  

Scaling: Applied Standard Scaling to ensure features like monthly_charges_inr and tenure_months are on a comparable scale. 

Train-Test Split: Divided the 2,000 records into an 80/20 split (1,600 for training, 400 for testing).  
