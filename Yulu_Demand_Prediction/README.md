# 🚲 Yulu: Micro-Mobility Demand Prediction Analysis

## Dataset:Columns
•	datetime: datetime

•	season: season (1: spring, 2: summer, 3: fall, 4: winter)

•	holiday: whether day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)

•	workingday: if day is neither weekend nor holiday is 1, otherwise is 0.

•	weather:

   o	1: Clear, Few clouds, partly cloudy, partly cloudy

   o	2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist

   o	3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds

   o	4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog

•	temp: temperature in Celsius

•	atemp: feeling temperature in Celsius

•	humidity: humidity

•	windspeed: wind speed

•	casual: count of casual users

•	registered: count of registered users

•	count: count of total rental bikes including both casual and registered


## 📌 Project Overview
Yulu is India's leading micro-mobility service provider, offering eco-friendly shared electric bi-cycles for urban commutes. In shared mobility, vehicle demand fluctuates drastically depending on weather conditions, working days, and seasonal trends. A shortage of bikes leads to lost revenue, while an oversupply causes high maintenance costs and operational inefficiencies.

The objective of this project is to perform a thorough **Exploratory Data Analysis (EDA)** and apply **Inferential Statistical Testing** on Yulu's ride data. This analysis uncovers how environmental variables and demographic factors affect bike sharing demand to optimize fleet management.

---

## 🚀 Key Analysis Frameworks & Deep Dives

### 1. Exploratory Data Analysis & Demand Profiling
▪️ **Temporal Demand Dynamics:** Mapping peak usage across hours, working vs. non-working days, and seasonal shifts.
▪️ **Weather Impact Matrix:** Profiling how different weather states (clear sky, mist, light rain, heavy rain) alter consumer adoption.
▪️ **Feature Engineering:** Extracting apparent temperature feeling indices and grouping hourly intervals into actionable operational shifts.

### 2. Inferential Statistical Testing
The core focus of this notebook is applying rigorous statistical frameworks to validate factors driving fleet demand:
🟢 **Two-Sample T-Tests:** Determining if working days vs. non-working days have a statistically significant impact on the mean number of rides.
🟡 **ANOVA (Analysis of Variance):** Testing if bike demand varies significantly across different seasons and weather classifications.
🔵 **Chi-Square Test of Independence:** Evaluating if weather states are dependent on the season, helping operations prepare for weather-based demand drops.

---

## 🛠️ Tech Stack & Methodology
* **Language:** Python
* **Statistical Modeling:** `scipy.stats` (T-tests, Levene's test for variance, Shapiro-Wilk test for normality, ANOVA, Chi-Square), `statsmodels`
* **Data Processing:** `pandas` (Datetime extraction, category re-mapping, aggregations), `numpy`
* **Visualization:** `seaborn`, `matplotlib` (Heatmaps, cyclical trend lines, box plots for variant distributions)

---

## 💻 How to Run This Project

### 1. Clone this repository
```bash
git clone https://github.com
cd yulu-demand-prediction
```

### 2. Install the required dependencies
Ensure your virtual environment is active, then install the packages:
```bash
pip install -r requirements.txt
```

### 3. Open the notebook
Launch the Jupyter framework to explore the mobility patterns and statistical validations:
```bash
jupyter notebook Yulu.ipynb
```

