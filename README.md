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

#Task 3 & 4: Neural Network Construction
Model Type: Sequential Feed-Forward Neural Network.

Design: Used 3 layers (16 neurons, 8 neurons, and 1 output neuron).

Training: Trained over 50 epochs.

Results: Observed the accuracy increasing as the model learned from the features.

#Task 5: Hyperparameter Experimentation
Experiment: Changed the Learning Rate from the default (0.001) to a slower rate (0.0001).

Observation: The original model reached high accuracy quickly, while the experimental model learned more slowly.

Conclusion: For this dataset, the default settings were effective, but experimentation is necessary to ensure the model doesn't "overfit" (memorize) the data.
