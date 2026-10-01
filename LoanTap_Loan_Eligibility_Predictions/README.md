# 🏦 LoanTap: Loan Eligibility Predictions & Repayment Terms

## Dataset:Columns
1.	loan_amnt : The listed amount of the loan applied for by the borrower. If at some point in time, the credit department reduces the loan amount, then it will be reflected in this value.

2.	term : The number of payments on the loan. Values are in months and can be either 36 or 60.

3.	int_rate : Interest Rate on the loan

4.	installment : The monthly payment owed by the borrower if the loan originates.

5.	grade : LoanTap assigned loan grade

6.	sub_grade : LoanTap assigned loan subgrade

7.	emp_title :The job title supplied by the Borrower when applying for the loan.

8.	emp_length : Employment length in years. Possible values are between 0 and 10 where 0 means less than one year and 10 means ten or more years.

9.	home_ownership : The home ownership status provided by the borrower during registration or obtained from the credit report.

10.	annual_inc : The self-reported annual income provided by the borrower during registration.

11.	verification_status : Indicates if income was verified by LoanTap, not verified, or if the income source was verified

12.	issue_d : The month which the loan was funded

13.	loan_status : Current status of the loan - Target Variable

14.	purpose : A category provided by the borrower for the loan request.

15.	title : The loan title provided by the borrower

16.	dti : A ratio calculated using the borrower’s total monthly debt payments on the total debt obligations, excluding mortgage and the requested LoanTap loan, divided by the borrower’s self-reported monthly income.

17.	earliest_cr_line :The month the borrower's earliest reported credit line was opened

18.	open_acc : The number of open credit lines in the borrower's credit file.

19.	pub_rec : Number of derogatory public records

20.	revol_bal : Total credit revolving balance

21.	revol_util : Revolving line utilization rate, or the amount of credit the borrower is using relative to all available revolving credit.

22.	total_acc : The total number of credit lines currently in the borrower's credit file

23.	initial_list_status : The initial listing status of the loan. Possible values are – W, F

24.	application_type : Indicates whether the loan is an individual application or a joint application with two co-borrowers

25.	mort_acc : Number of mortgage accounts.

26.	pub_rec_bankruptcies : Number of public record bankruptcies

27.	Address: Address of the individual


## 📌 Project Overview
LoanTap is a premier FinTech platform offering customized loan products to salaried professionals. In consumer lending, balancing loan approvals with credit risk underwriting is paramount. Approving high-risk individuals leads to non-performing assets (NPAs), while over-tightening criteria results in lost revenue and poor customer acquisition.

The objective of this project is to build an end-to-end **Predictive Classification Pipeline** that determines whether a loan applicant should be approved, while evaluating optimal repayment terms and credit risk profiling to minimize financial default rates.

---

## 🚀 Key Analysis Frameworks & Modeling Pipeline

### 1. Exploratory Data Analysis & Risk Metrics
▪️ **Credit Underwriting Factors:** Evaluating the impact of debt-to-income (DTI) ratios, revolving utilization rates, and credit history length on approval rates.
▪️ **Employment & Income Profiling:** Correlating employment titles, lengths of service, and annual income against historical default vectors.
▪️ **Class Imbalance Diagnostics:** Identifying structural data skewness where loan defaulters represent a minority class, requiring targeted sampling adjustments.

### 2. Predictive Modeling & Evaluation
The repository steps through multiple machine learning models optimized for financial precision:
🟢 **Baseline Classifier:** Logistic Regression to uncover structural feature weights and odds ratios.
🟡 **Tree-Based Models:** Random Forests and Gradient Boosting architectures to capture non-linear relationships.
🔵 **Evaluation Metrics:** Prioritizing precision-recall curves, ROC-AUC metrics, and custom threshold tuning to strictly control **False Positives** (approving high-risk borrowers).

---

## 🛠️ Tech Stack & Methodology
* **Language:** Python
* **Machine Learning:** `scikit-learn` (Logistic Regression, Random Forest, GridSearchCV, Precision-Recall Metrics)
* **Imbalance Handling:** `imbalanced-learn` (SMOTE / Undersampling configurations if applicable)
* **Data Engineering:** `pandas` (One-hot encoding, binning continuous variables, continuous value transformations), `numpy`
* **Visualization:** `seaborn`, `matplotlib` (Confusion matrices, ROC curves, feature importance ranking)

---

## 💻 How to Run This Project

### 1. Clone this repository
```bash
git clone https://github.com
cd loantap-eligibility-predictions
```

### 2. Install the required dependencies
Ensure your virtual environment is active, then install the packages:
```bash
pip install -r requirements.txt
```

### 3. Open the notebook
Launch the Jupyter interface to step through the underwriting logic and predictive models:
```bash
jupyter notebook LoanTap_case_study.ipynb
```

   ```
