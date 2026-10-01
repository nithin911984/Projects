# 🎓 Ivy League College Admission Prediction

<img src="https://shields.io" alt="Dataset" valign="middle"> <img src="https://shields.io" alt="Domain" valign="middle"> <img src="https://shields.io" alt="Task" valign="middle">

•	Serial No. (Unique row ID)
•	GRE Scores (out of 340)
•	TOEFL Scores (out of 120)
•	University Rating (out of 5)
•	Statement of Purpose and Letter of Recommendation Strength (out of 5)
•	Undergraduate GPA (out of 10)
•	Research Experience (either 0 or 1)
•	Chance of Admit (ranging from 0 to 1)

## 📌 Project Overview
Jamboree is a leading EdTech platform helping students secure admissions to premium international universities. Navigating the highly competitive Ivy League and top-tier global university admission process is challenging for applicants who want to know where they stand based on their academic profiles.

The objective of this project is to analyze the Jamboree dataset, identify the most critical factors influencing university acceptance, and build a highly accurate **Predictive Regression Model** to estimate a student's probability of admission.

---

## 🚀 Key Analysis & Modeling Frameworks

### 1. Exploratory Data Analysis & Feature Insights
▪️ **Academic Weightage:** Analyzing the impact of core standardized tests (GRE, TOEFL scores) vs. cumulative GPA (CGPA).
▪️ **Qualitative Strength:** Evaluating the correlation between subjective features like Statement of Purpose (SOP), Letters of Recommendation (LOR), and Research Experience.
▪️ **Multicollinearity Diagnostics:** Using Variance Inflation Factor (VIF) to detect and resolve highly correlated independent variables.

### 2. Predictive Modeling Pipeline
The analysis evaluates regression architectures to establish accurate prediction parameters:
🟢 **Baseline Model:** Ordinary Least Squares (OLS) Linear Regression to evaluate structural feature coefficients.
🟡 **Regularized Regression:** Implementing Ridge and Lasso Regression to prevent overfitting and handle feature penalty weightings.
🔵 **Assumption Testing:** Validating linear regression assumptions including Homoscedasticity, Normality of Residuals (Q-Q plots), and Independence of Errors.

---

## 🛠️ Tech Stack & Methodology
* **Language:** Python
* **Machine Learning & Stats:** `scikit-learn` (Linear Regression, Ridge, Lasso, Train-Test Split), `statsmodels` (OLS summary, VIF analysis)
* **Data Wrangling:** `pandas`, `numpy`
* **Visualization:** `seaborn`, `matplotlib` (Residual plots, correlation heatmaps, feature importance graphs)

---

## 💻 How to Run This Project

### 1. Clone this repository
```bash
git clone https://github.com
cd ivy-league-admission-prediction
```

### 2. Install the required dependencies
Ensure your virtual environment is active, then run:
```bash
pip install -r requirements.txt
```

### 3. Open the notebook
Launch the Jupyter framework to step through the dataset analysis, statistical tests, and models:
```bash
jupyter notebook Jamboree_Case_Study.ipynb
```

   ```
