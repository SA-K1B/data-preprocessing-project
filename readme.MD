# Loan Application Dataset Preprocessing

## Introduction
This project aims to preprocess loan application data to prepare it for further analysis or modeling. The preprocessing steps include handling missing values, encoding categorical variables, and splitting the dataset into training and testing sets.

## Dataset
The dataset used in this project is `data.csv`, which contains various features related to loan applications, including:
- Loan_ID
- Gender
- Married
- Dependents
- Education
- Self_Employed
- ApplicantIncome
- CoapplicantIncome
- LoanAmount
- Loan_Amount_Term
- Credit_History
- Property_Area
- Loan_Status

## Preprocessing Steps
1. **Load the dataset**: The dataset is loaded using Pandas.
2. **Drop Loan_ID column**: The `Loan_ID` column is dropped as it is not needed for analysis.
3. **Check for missing values**: The script checks for any missing values in the dataset.
4. **Split the dataset**: The dataset is split into training and testing sets, with `Loan_Status` as the target variable.
5. **Fill missing values**:
   - For `LoanAmount` and `Loan_Amount_Term`, missing values are filled with the mean of the respective columns.
   - For categorical columns (`Gender`, `Married`, `Dependents`, `Self_Employed`, `Credit_History`), missing values are filled with the mode.
6. **Convert categorical variables**: Categorical columns are converted to numerical values using one-hot encoding.
7. **Map target variable**: The target variable `Loan_Status` is mapped to numerical values (1 for 'Y' and 0 for 'N').

## Usage
To run the preprocessing script, execute the `preprocessing.ipynb` file in a Jupyter Notebook environment.

## Conclusion
The preprocessing steps are crucial for preparing the data for further analysis or machine learning modeling. Proper handling of missing values and encoding of categorical variables ensures that the dataset is ready for use in predictive modeling.
