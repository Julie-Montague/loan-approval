# Loan Approval Prediction Using Python and Machine Learning

## 1. Project Overview
This project demonstrates an end-to-end data science workflow using Python to predict whether a loan application will be approved or rejected. The project uses structured loan application data and applies exploratory data analysis, data preprocessing, feature transformation, class imbalance handling, supervised machine learning, and model evaluation.


## 2. Objectives
The objectives of this project are to:
  1. Understand the structure and quality of the loan approval dataset.
  2. Analyze applicant, financial, credit history, and loan-related variables.
  3. Prepare the dataset for machine learning through cleaning, encoding, and transformation.
  4. Address class imbalance using resampling techniques.
  5. Train and compare multiple supervised classification models.
  6. Evaluate model performance using appropriate classification metrics.
  7. Present the workflow and results in a clear technical portfolio format.

## 3. Technical Focus
This project highlights the use of Python as a data processing language for a machine learning task. Python was used to:

  -  Load and inspect structured tabular data.
  -  Explore numerical and categorical variables.
  -  Clean and transform raw features.
  -  Encode categorical variables for machine learning.
  -  Handle outliers and class imbalance.
  -  Train and compare classification models.
  -  Evaluate model performance using standard classification metrics.
  -  Document results in a clear and reproducible format.

## 4. Dataset Description
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
| Category | Tools | 
|---|---:|---:|
| Programming Language | Python |
| Data Processing | Pandas, Numpy |
| Data Visualization | Matplotlib, Seaborn |
| Machine Learning | Matplotlib, Seaborn |
| Development Environment | Jupyter Notebook |
| Version Control | Git, Github |

## 5. Project Workflow

The implementation is organized into two main notebooks:
  1. Exploratory Data Analysis
Focuses on understanding the dataset, visualizing feature distributions, checking relationships between variables, and identifying potential data quality issues.
  2. Preprocessing and Modelling
Focuses on preparing the dataset for machine learning, training classification models, evaluating performance, and comparing results.

### 5.1 Exploratory Data Analysis

Notebook link : ![EDA Notebook](https://github.com/Julie-Montague/loan-approval/blob/main/Exploratory%20Data%20Analysis.ipynb)

The exploratory notebook focuses on understanding the dataset before modelling. This included:

  - Checking dataset shape, column names, and data types.
  - Reviewing summary statistics for numerical variables.
  - Exploring categorical variable distributions.
  - Analyzing the distribution of the target variable.
  - Comparing loan approval outcomes across applicant and loan characteristics.
  - Creating visualizations to identify patterns in income, credit score, loan amount, loan intent, and previous default history.
  - Checking correlations between numerical variables.
  - Identifying potential outliers and unusual values.
    
Summary Findings :
  - The data did not have any missing values or duplicated rows
  - Using **Interquartile Range Method**, some of the numerical outliers showeed presence of extreme values which led to implementation of outlier handling
  - Using **Variance Inflation Factor**, `person_age` had a very high factor of 156


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
