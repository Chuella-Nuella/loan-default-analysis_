Loan Default Analysis - Milestone 1 (EDA)
This repository contains Milestone 1: Exploratory Data Analysis (EDA) for the Loan Default Prediction Project based on the Loan_default.csv dataset from Kaggle.
The goal of this milestone is to clean, explore, preprocess, and prepare the dataset for machine-learning modeling in later milestones.
Overview of the Project
Examples of microfinance institutions that heavily rely on data-driven risk assessment to make informed lending decisions include LAPO Microfinance Bank.
The following project does an extensive EDA on the loan dataset to find:
• Key borrower risk factors
• Patterns related to loan defaults
• Relevant numerical and categorical relationships
• Outliers and data quality issues
•	Features to be used in Predictive Modelling
Dataset Information - Narrative Format
Features of this dataset are as follows:
Age -- The age of each borrower.
Income – The annual income of the borrower.
CreditScore - The creditworthiness score of the borrower.
MonthsEmployed - Number of months the borrower has been employed.
NumCreditLines – The total number of active credit lines the borrower has.
InterestRate - The interest rate applied to the borrower's loan.
LoanTerm- The duration or repayment period of the loan.
DTIRatio – The borrower's debt-to-income ratio.
EmploymentType - The type or category of employment of the borrower.
MaritalStatus: The marital status of the borrower.
HasMortgage - Indicates whether the borrower has an active mortgage.
HasDependents - Indicates if the borrower has dependents.
Steps Performed in the Notebook
1. Load Dataset
Loaded using pandas.read_csv() from a local path.
 2. Dataset Overview
Displayed:
•	.head()
•	.info()
•	.describe()
 3. Missing Values
Computed missing values per column.
 4. Data Cleaning
•	Numeric missing values → median
•	Categorical missing values → mode
•	Dropped LoanID
•	Removed outliers using Winsorization
 5. Feature Engineering
Added:
•	Income_to_Loan (financial stability indicator)
•	Employment_Stability (binary employment duration flag)
6. Outlier Handling
Winsorized the major numeric columns.
7. Encoding
Used LabelEncoder for memory-efficient encoding of categorical variables.
 8. Correlation Analysis
Generated a heatmap of correlations between features.
 9. Export Cleaned Dataset
Saved cleaned file to:
C:\Users\wuser\OneDrive - Nexford University\New Folder\loan_default_cleaned.csv
Visualizations Included
•	Correlation Heatmap
•	Boxplots for outliers
•	Distribution plots for numeric features
•	Count plots for categorical variables
(As included or later added in the notebook)
Repository Structure
loan-default-analysis
 ┣  loan-default-analysis.ipynb        # Main EDA notebook
 ┣  loan_default_cleaned.csv           # Cleaned dataset 
 ┣ README.md                           # Project documentation
 ┗  assets/                             # Optional images/plots
How to Run This Project
1. Install Requirements
pip install pandas numpy matplotlib seaborn scikit-learn
2. Open Jupyter Notebook
jupyter notebook
3. Run the Notebook
Open:
loan-default-analysis.ipynb

Saving the Cleaned Dataset
You used the code:
output_path = r"C:\Users\wuser\OneDrive - Nexford University\New Folder\loan_default_cleaned.csv"
df.to_csv(output_path, index=False) This will save the cleaned dataset in your specified folder.







# loan-default-analysis_
