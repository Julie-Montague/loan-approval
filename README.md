# LOAN APPROVAL PREDICTION
# OVERVIEW
This is a supervised machine learning project that uses the kaggle loan approval dataset to compare several models' performance. The goal is to compare different machine learning models to achieve the highest model performance during prediction.
# DATASET
The dataset is can be obtained from Kaggle and contains variables of different features taken into account during the loan approval process are used to predict if a loan application will be approved or rejected.
# Feature Description
   - Person_Age - The age of the person - Float
   - person_gender - Gender of the person - Categorical
   - person_education - Highest education level - Categorical
   - person_income - Annual income - Float
   - person_emp_exp - Years of employment experience - Integer
   - person_home_ownership - Home ownership status (e.g., rent, own, mortgage) - Categorical
   - loan_amnt - Loan amount requested - Float
   - loan_intent - Purpose of the loan - Categorical
   - loan_int_rate - Loan interest rate - Float
   - loan_percent_income - Loan amount as a percentage of annual income - Float
   - cb_person_cred_hist_length - Length of credit history in years - Float
   - credit_score - Credit score of the person - Integer
   - previous_loan_defaults_on_file - Indicator of previous loan defaults - Categorical
   - loan_status (target variable) - Loan approval status: 1 = approved; 0 = rejected - Integer
# NOTEBOOK STRUCTURE
1. Exploratoty Data Analysis Notebook:
     - Categorical data EDA
     - Numerical data EDA
     - Correlation plots
     - Monotonicity Check ( Binned X-Y visuals, spearman correlation, PDP-plots)
     - Outliers check
2. Preprocess & Modelling Notebook:
     - Data Pre-processing :
         - handle missing values ifany
         - check for duplicates
         - reduce categories ifnot enough data
         - encode categorical data
         - Handle outliers
    - Train-Test Split
    - Resampling
    - Modelling (Random Forest, Decision Trees, LightGBM, GradientBoosting,K-Nearest Neighbors,Naive Bayes Classifier)
     
