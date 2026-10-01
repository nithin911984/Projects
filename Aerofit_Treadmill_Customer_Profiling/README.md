# Aerofit Treadmill: Customer Profiling & Case Study

# Dataset : Columns
* Product: Product Purchased KP281, KP481, or KP781
* Age: In years
* Gender: Male/Female
* Education: in years
* MaritalStatus: single or partnered
* Usage: average number of times the customer plans to use the treadmill each week
* Income: annual income (in $)
* Fitness: self-rated fitness on a 1-to-5 scale, where 1 is poor shape and 5 is the
excellent shape
* Miles: average number of miles the customer expects to walk/run each week

## 📌 Project Overview
Aerofit is a leading brand in fitness equipment. The market research team wants to identify the characteristics of the target audience for each type of treadmill offered by the company to provide better product recommendations to new customers.

The objective of this project is to perform an Exploratory Data Analysis (EDA) on raw customer data to construct detailed customer profiles and calculate conditional probabilities for product purchases.

## 📊 The Product Line
* KP281: Entry-level treadmill ($1,500) - For beginners.
* KP481: Mid-level treadmill ($1,750) - For intermediate runners.
* KP781: Premium treadmill ($2,500) - For advanced/heavy fitness users.

## 🚀 Key Insights Uncovered
* Income Thresholds: Customers with an annual income over $60,000 almost exclusively purchase the premium KP781 model.
* Gender Distributions: The KP781 model shows a heavy skew toward male buyers, while the KP281 and KP481 models are evenly distributed among all genders.
* Fitness Correlation: Users who rate their fitness levels as 4 or 5 out of 5 have an incredibly high probability of purchasing the KP781 model.

## 🛠️ Tech Stack & Methodology
* Language: Python
* Libraries: Pandas (Data Cleaning), Seaborn & Matplotlib (Data Visualization), NumPy (Analytical operations).
* Techniques: Contingency tables, Marginal & Conditional Probability distribution analysis, Outlier detection.

## 💻 How to Run This Project
1. Clone this repository:
   ```bash
   git clone https://github.com
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the notebook:
   ```bash
   jupyter notebook Aerofit_treadmill_casestudy.ipynb
   ```

