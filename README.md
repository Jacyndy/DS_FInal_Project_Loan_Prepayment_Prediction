# DS_Final_Project_Loan_Prepayment_Prediction

# Objectives
Predict the age of loans to better understand early prepayment patterns and borrower behavior.

# Why It Matters
Helps lenders anticipate borrower behavior.
Supports risk management.
Improves prepayment forecasting.

# Data Source and Variables
Dataset: Lending Club (from Kaggle).
Target Variable: Loan age.
Key Features: Loan amount, installment, total payment, last payment amount, purpose, home ownership, open accounts. 

# Data Prep and Feature Engineering
Handled missing values.
Feature engineering: 
Engineered loan age = last payment date – issue date  and filtered out all paid out loans in number of months.
Encoded categorical variables.

# Exploratory Data Analysis
some of the relationships shown in the the notebook:
![int_rate vs loan_age](images/output4.png) 
![installement vs loan_age](images/output.png) 
![open_acc vs loan_age](images/output2.png) 
![Funded_amount vs Loan_age](images/output3.png)

# Results
![Results](images/results.png)

# Interpretation
Last payment amount shows the strongest correlation with loan age.
Most features are statistically significant.
Negative relationships: loan amount, interest rate, monthly installment, annual income, open accounts, purpose.
Positive relationship: home ownership.

# Challenges and Future Works
## Challenges:
Limited dataset size restricted deeper model training.
Runtime constraints when experimenting with complex algorithms.
## Future Work:
Consider time series analysis and extend model to include macroeconomic indicators.
Deploy as a web app for real-time prediction to be used by underwriters.
Combine with prepayment prediction for end-to-end forecasting.
