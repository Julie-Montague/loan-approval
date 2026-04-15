# Loan Approval Prediction Using Machine Learning

## 1. Project Overview
This project applies supervised machine learning to predict whether a loan application will be approved or rejected. The project demonstrates an end-to-end data science workflow, including data exploration, preprocessing, feature encoding, resampling, model training, and model comparison.

The main goal is to use applicant demographic, financial, credit history, and loan-related information to build classification models that can support loan approval prediction.

## 2. Objectives
- Explore the structure and quality of the loan approval dataset.
- Identify important patterns in applicant income, credit score, loan amount, loan intent, and previous default history.
- Prepare the dataset for machine learning through cleaning, encoding, outlier handling, and resampling.
- Train and compare multiple classification models.
- Select the best-performing model based on evaluation metrics.

## 3. Dataset Description
The dataset contains loan application records with applicant, financial, and credit-related variables.

### Target Variable
- `loan_status`: Loan approval status  
  - `1` = Approved  
  - `0` = Rejected
![Target Distrbution](images/target_distribution.png)

### Main Features
- `person_age`: Applicant age
- `person_gender`: Applicant gender
- `person_education`: Highest education level
- `person_income`: Annual income
- `person_emp_exp`: Employment experience
- `person_home_ownership`: Home ownership status
- `loan_amnt`: Loan amount requested
- `loan_intent`: Purpose of the loan
- `loan_int_rate`: Loan interest rate
- `loan_percent_income`: Loan amount as a percentage of income
- `cb_person_cred_hist_length`: Credit history length
- `credit_score`: Applicant credit score
- `previous_loan_defaults_on_file`: Previous default history

## 4. Tools and Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- LightGBM
- Matplotlib
- Seaborn
- Jupyter Notebook

## 5. Project Workflow

The project was completed in two main stages:

### 5.1 Exploratory Data Analysis
The EDA notebook focuses on understanding the dataset before modelling. This included:

- Checking the shape and structure of the dataset.
- Exploring categorical and numerical variables.
- Visualizing feature distributions.
- Analyzing the target variable distribution.
- Checking relationships between features and loan approval status.
- Creating correlation plots.
- Checking monotonic relationships using binned visualizations, Spearman correlation, and partial dependence plots.
- Identifying potential outliers.

### 5.2 Data Preprocessing and Modelling
The preprocessing and modelling notebook prepares the data for machine learning. This included:

- Checking and handling missing values.
- Checking duplicate records.
- Reducing rare categories where necessary.
- Encoding categorical variables.
- Handling outliers.
- Splitting the data into training and testing sets.
- Applying resampling techniques to address class imbalance.
- Training and comparing multiple classification models.

## 6. Machine Learning Models Compared
The following models were trained and evaluated:

- Random Forest Classifier
- Decision Tree Classifier
- LightGBM Classifier
- Gradient Boosting Classifier
- K-Nearest Neighbors
- Naive Bayes Classifier

## 7. Evaluation Approach
Model performance was evaluated using classification metrics such as:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

Since loan approval prediction may involve class imbalance, F1-score and recall are especially useful because they provide more information than accuracy alone.

## 8. Key Results

![Model Comparison](images/model_comparison.png)

Add a table like this:

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| Random Forest | Add value | Add value | Add value | Add value |
| Decision Tree | Add value | Add value | Add value | Add value |
| LightGBM | Add value | Add value | Add value | Add value |
| Gradient Boosting | Add value | Add value | Add value | Add value |
| KNN | Add value | Add value | Add value | Add value |
| Naive Bayes | Add value | Add value | Add value | Add value |

## 9. Skills Demonstrated
This project demonstrates the following technical skills:

### Data Processing
- Loaded and explored structured tabular data using Python.
- Cleaned the dataset by checking missing values, duplicates, and inconsistent categories.
- Encoded categorical variables for machine learning models.
- Handled outliers and prepared numerical features.
- Applied resampling techniques to address class imbalance.

### Exploratory Data Analysis
- Analyzed categorical and numerical variables.
- Created distribution plots and correlation visualizations.
- Investigated relationships between loan applicant features and approval outcomes.
- Used visual analysis to support preprocessing and modelling decisions.

### Machine Learning
- Built a supervised classification pipeline.
- Compared multiple machine learning models.
- Evaluated models using classification metrics.
- Interpreted model performance to identify the strongest approach.

### Portfolio and Documentation
- Organized the project into separate notebooks for EDA and modelling.
- Documented the dataset, workflow, tools, models, and results.
- Presented the project in a clear format suitable for technical review.

## 10. Project Files
```text
loan-approval/
│
├── Exploratory Data Analysis.ipynb
├── Preprocess & Modelling.ipynb
├── loan_data.csv
├── README.md
└── images/
    ├── target_distribution.png
    └── model_comparison.png
