# 🚖 Ola: Driver Churn Predictions & Retention Analysis

## Dataset:Columns
1.	MMMM-YY : Reporting Date (Monthly)
2.	Driver_ID : Unique id for drivers
3.	Age : Age of the driver
4.	Gender : Gender of the driver – Male : 0, Female: 1
5.	City : City Code of the driver
6.	Education_Level : Education level – 0 for 10+ ,1 for 12+ ,2 for graduate
7.	Income : Monthly average Income of the driver
8.	Date Of Joining : Joining date for the driver
9.	LastWorkingDate : Last date of working for the driver
10. Joining Designation : Designation of the driver at the time of joining
11. Grade : Grade of the driver at the time of reporting
12. Total Business Value : The total business value acquired by the driver in a month (negative business indicates cancellation/refund or car EMI adjustments)
13. Quarterly Rating : Quarterly rating of the driver: 1,2,3,4,5 (higher is better)


## 📌 Project Overview
Ola is a leading global ridesharing platform. In the gig economy, driver churn (attrition) is a critical bottleneck that directly impacts supply consistency, ride wait times, and customer satisfaction. Recruiting new drivers is significantly more expensive than retaining existing ones, making early churn detection highly valuable.

The objective of this project is to build an end-to-end **Predictive Classification Pipeline** that determines whether a driver is likely to churn. By engineering features from historical performance records, this study helps the operations team implement targeted retention strategies.

---

## 🚀 Key Analysis Frameworks & Modeling Pipeline

### 1. Data Aggregation & Feature Engineering
▪️ **Temporal Reconstructions:** Aggregating granular, multi-row monthly records for each driver to build historical performance timelines.
▪️ **KPI Extraction:** Engineering core performance markers including quarterly rating changes, income growth trends, and monthly delivery/ride volume drops.
▪️ **Driver Class Labeling:** Programmatically identifying churn vectors based on missing updates or explicit termination indicators in the data timeline.

### 2. Predictive Modeling & Class Imbalance
The notebook explores machine learning pipelines optimized for handling behavioral tracking:
🟢 **Baseline Classifier:** Logistic Regression to map baseline linear dependencies and structural feature weights.
🟡 **Ensemble Models:** Random Forests and LightGBM / XGBoost architectures to evaluate complex, non-linear churn indicators.
🔵 **Imbalance Diagnostics:** Utilizing techniques like SMOTE or class weighting to compensate for the fact that churned drivers represent a minority segment.

---

## 🛠️ Tech Stack & Methodology
* **Language:** Python
* **Machine Learning:** `scikit-learn` (Ensemble classifiers, GridSearchCV, Precision-Recall tuning), `xgboost` / `lightgbm` (if applicable)
* **Data Processing:** `pandas` (Complex grouping, row-to-column aggregations, rolling metrics), `numpy`
* **Visualization:** `seaborn`, `matplotlib` (Correlation matrices, ROC curves, feature importance bar charts)

---

## 💻 How to Run This Project

### 1. Clone this repository
```bash
git clone https://github.com
cd ola-driver-churn
```

### 2. Install the required dependencies
Ensure your virtual environment is active, then install the packages:
```bash
pip install -r requirements.txt
```

### 3. Open the notebook
Launch the Jupyter framework to explore the driver behavior tracking and churn model pipeline:
```bash
jupyter notebook Ola_driver_churn.ipynb
```

   ```
