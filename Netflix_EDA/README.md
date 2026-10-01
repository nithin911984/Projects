# 🎬 Netflix: Exploratory Data Analysis Case Study

## Dataset : Columns
* Title: Title of the Movie / Tv Show
* Director: Director of the Movie
* Cast: Actors involved in the movie/show
* Country: Country where the movie/show was produced
* Date_added: Date it was added on Netflix
* Release_year: Actual Release year of the movie/show
* Rating: TV Rating of the movie/show
* Duration: Total Duration - in minutes or number of seasons
* Listed_in: Genre
* Description: The summary description

## 📌 Project Overview
Netflix is one of the world's leading entertainment services with over 200 million paid memberships. Their massive media catalog is constantly shifting as they produce original content and license global titles. Understanding content distribution, regional trends, release cycles, and category configurations is vital for tailoring future user acquisition strategies.

The objective of this project is to perform an extensive **Exploratory Data Analysis (EDA)** on the Netflix dataset. By clean-parsing structural components and parsing multi-valued attributes, this analysis uncovers actionable business insights regarding Netflix's content ecosystem.

---

## 🚀 Key Analysis Frameworks & Deep Dives

### 1. Data Cleaning & Unnesting
▪️ **Handling Multi-valued Attributes:** Advanced unnesting of categorical strings to accurately evaluate fields like `cast`, `director`, `country`, and `listed_in`.
▪️ **Temporal Extraction:** Parsing dates to isolate upload years, months, and weekdays to discover platform content scheduling patterns.
▪️ **Missing Value Strategies:** Analyzing missing fields across critical content markers and applying data-driven imputation rules.

### 2. Analytical Segmentation & Trends
🟢 **Content Split:** Comparing the operational growth and volume trajectories of Movies versus TV Shows.
🟡 **Geographical Footprint:** Tracking content production powerhouses by isolating country data to identify top global contributors.
🔵 **Text & Genre Deep Dive:** Grouping ratings, runtimes, and genre tags (`listed_in`) to profile Netflix's target audience segments.

---

## 🛠️ Tech Stack & Methodology
* **Language:** Python
* **Data Manipulation:** `pandas` (String manipulation, unnesting arrays, custom aggregations), `numpy`
* **Data Visualization:** `seaborn`, `matplotlib` (Word clouds, horizontal bar plots, dual-axis growth charts, stacked trend plots)
* **Statistical Profiling:** Distribution metrics, categorical counts, and historical trend analyses.

---

## 💻 How to Run This Project

### 1. Clone this repository
```bash
git clone https://github.com
cd netflix-eda-project
```

### 2. Install the required dependencies
Ensure your virtual environment is active, then install the packages:
```bash
pip install -r requirements.txt
```

### 3. Open the notebook
Launch the Jupyter framework to explore the visual data deep dive:
```bash
jupyter notebook Netflix_EDA.ipynb
```

   ```
