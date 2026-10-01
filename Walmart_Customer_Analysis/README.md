# 🛒 Walmart: Customer Purchase Behaviour Analysis

## 📌 Project Overview
Walmart is the world's largest multinational retail corporation, managing massive transaction volumes daily. Optimizing inventory management, targeted marketing, and product placements depends heavily on understanding user buying habits across different demographic segments.

The objective of this project is to analyze transaction data to dissect **customer purchase behavior**. By combining rigorous Exploratory Data Analysis (EDA) with **inferential statistical analysis**, this study uncovers how demographic attributes—such as gender, age, and marital status—impact consumer spending habits.

---

## 🚀 Key Analysis Frameworks & Deep Dives

### 1. Exploratory Data Analysis & Customer Segmentation
▪️ **Demographic Spending Profiles:** Segmenting purchase volumes across gender, age groups, city tiers, and occupations.
▪️ **Product Category Volume:** Identifying high-traction product categories and evaluating customer product affinity maps.
▪️ **Outlier Treatment:** Detecting anomalous transactions and handling heavy-tailed purchase data distributions.

### 2. Inferential Statistical Testing
The core of this notebook uses statistical frameworks to validate data patterns and avoid false correlations:
🟢 **Central Limit Theorem (CLT):** Demonstrating how the distribution of sample means approaches normality as sample size increases, enabling parametric calculations.
🟡 **Hypothesis Testing (Gender & Marriage):** Using T-tests or Z-tests to mathematically verify whether spending habits differ significantly between male vs. female and married vs. single buyers.
🔵 **Multi-Class Variances:** Utilizing ANOVA or Chi-Square tests to evaluate variance across age brackets and city categories.

---

## 🛠️ Tech Stack & Methodology
* **Language:** Python
* **Statistical Modeling:** `scipy.stats` (T-tests, Z-tests, ANOVA, Normality tests, CLT simulations), `statsmodels`
* **Data Processing:** `pandas` (Binning, demographic mapping, group aggregations), `numpy`
* **Visualization:** `seaborn`, `matplotlib` (Density plots, box plots for distribution spreads, bar grids)

---

## 💻 How to Run This Project

### 1. Clone this repository
```bash
git clone https://github.com
cd walmart-purchase-behavior
```

### 2. Install the required dependencies
Ensure your virtual environment is active, then install the packages:
```bash
pip install -r requirements.txt
```

### 3. Open the notebook
Launch the Jupyter ecosystem to explore the full demographic breakdown and statistical validations:
```bash
jupyter notebook Walmart_case_study.ipynb
```

   ```
