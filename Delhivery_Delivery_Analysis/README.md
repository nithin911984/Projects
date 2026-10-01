# 🚚 Delhivery: Logistics Delivery Analysis & Strategy Building

<img src="https://shields.io" alt="Dataset" valign="middle"> <img src="https://shields.io" alt="Industry" valign="middle"> <img src="https://shields.io" alt="Task" valign="middle">

## 📌 Project Overview
Delhivery is India's largest fully integrated logistics services provider. To maintain high efficiency and outpace competitors, the company relies heavily on data-driven intelligence to forecast delivery times, optimize shipping routes, and minimize delays between warehouses and final destinations.

The objective of this project is to clean, process, and analyze raw logistics data from Delhivery. By engineering key features and analyzing delivery time gaps, this study provides actionable strategic recommendations to optimize transit operations and improve supply chain predictability.

---

## 🚀 Key Analysis Frameworks & Strategy Blocks

### 1. Data Cleaning & Structuring
▪️ **Handling Aggregated Data:** Managing raw telemetry logs by parsing and reconstructing trips from source to destination.
▪️ **Outlier Detection:** Identifying anomalies in distance and time metrics using statistical techniques (IQR) to flag exceptional delays.
▪️ **Missing Value Imputation:** Resolving missing data elements in spatial and temporal features to ensure data integrity.

### 2. Feature Engineering & Discrepancy Analysis
🟢 **Time Gaps:** Analyzing the variance between Actual Transit Time and the Open Source Routing Machine (OSRM) predicted time.
🟡 **Distance Gaps:** Comparing actual kilometers traveled against OSRM-computed shortest paths to track routing inefficiencies.
🔵 **Categorical Engineering:** Grouping delivery points by state, city tiers, and route types (FTL vs. Carting) to pinpoint structural bottlenecks.

---

## 🛠️ Tech Stack & Methodology
* **Language:** Python
* **Data Manipulation:** `pandas` (Grouping, aggregations, datetime parsing, data type conversions), `numpy`
* **Data Visualization:** `seaborn`, `matplotlib` (Distribution plots, box plots for outlier tracking)
* **Statistical Analysis:** Hypothesis testing (ks_2samp) to validate differences between actual_distance and estimated_distance

---

## 💻 How to Run This Project

### 1. Clone this repository
```bash
git clone https://github.com
cd delhivery-delivery-analysis
```

### 2. Install the required dependencies
Ensure your virtual environment is active, then install the packages:
```bash
pip install -r requirements.txt
```

### 3. Open the notebook
Launch the Jupyter framework to explore the full analysis and strategic takeaways:
```bash
jupyter notebook Delhivery_Case_Study.ipynb
```

