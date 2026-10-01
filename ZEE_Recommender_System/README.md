# 🎬 Zee: Personalized Content Recommender System

## Dataset:Ratings:Columns

UserID::MovieID::Rating::Timestamp

•	UserIDs range between 1 and 6040

•	MovieIDs range between 1 and 3952

•	Ratings are made on a 5-star scale (whole-star ratings only)

•	Timestamp is represented in seconds

•	Each user has at least 20 ratings

## Dataset:Users:Columns

•	Gender is denoted by a "M" for male and "F" for female

•	Age is chosen from the following ranges:

   o	1: "Under 18"

   o	18: "18-24"

   o	25: "25-34"

   o	35: "35-44"

   o	45: "45-49"

   o	50: "50-55"

   o	56: "56+"

•	Occupation is chosen from the following choices:

   o	0: "other" or not specified

   o	1: "academic/educator"

   o	2: "artist"

   o	3: "clerical/admin"

   o	4: "college/grad student"

   o	5: "customer service"

   o	6: "doctor/health care"

   o	7: "executive/managerial"

   o	8: "farmer"

   o	9: "homemaker"

   o	10: "K-12 student"

   o	11: "lawyer"

   o	12: "programmer"

   o	13: "retired"

   o	14: "sales/marketing"

   o	15: "scientist"

   o	16: "self-employed"

   o	17: "technician/engineer"

   o	18: "tradesman/craftsman"

   o	19: "unemployed"

   o	20: "writer"

## Dataset:Movies:Columns

•	Titles are identical to titles provided by the IMDB (including year of release)

•	Genres are pipe-separated and are selected from the following genres:

   o	Action
   
   o	Adventure

   o	Animation

   o	Children's

   o	Comedy

   o	Crime

   o	Documentary

   o	Drama

   o	Fantasy

   o	Film-Noir

   o	Horror

   o	Musical

   o	Mystery

   o	Romance

   o	Sci-Fi

   o	Thriller

   o	War

   o	Western

## 📌 Project Overview
Zee Entertainment is a global media and entertainment powerhouse with an expansive content library. In modern digital streaming, user engagement and retention depend entirely on serving highly accurate, personalized suggestions. Finding content blindly leads to churn, whereas predictive personalization boosts watch time and customer satisfaction.

The objective of this project is to build an end-to-end **Content Recommendation Pipeline**. By exploring user streaming behavior, item profiles, and historical ratings, this notebook implements and evaluates multiple filtering strategies to optimize user discovery.

---

## 🚀 Key Analysis Frameworks & Recommendation Engines

### 1. Exploratory Data Analysis & Sparsity Mapping
▪️ **User-Item Interaction Profiles:** Analyzing the distribution of ratings, identifying power users, and tracking long-tail content items.
▪️ **Sparsity Diagnostics:** Calculating the interaction matrix density to assess the scope of the cold-start problem.
▪️ **Temporal Consumptions:** Dissecting seasonal patterns, genre popularity shifts, and watch-time cyclicality.

### 2. Algorithmic Modeling Architectures
The notebook walks through the development and comparison of multiple recommendation paradigms:
🟢 **Popularity-Based Engine:** Baseline model recommending top-rated, trending content globally to handle new user cold-starts.
🟡 **Content-Based Filtering:** Building item profile vectors using metadata features (genres, directors, cast) to recommend similar content based on user watch histories.
🔵 **Collaborative Filtering:** Implementing item-item or user-user matrix factorization techniques (such as Cosine Similarity, Pearson Correlation, or Singular Value Decomposition) to capture latent user patterns.

---

## 🛠️ Tech Stack & Methodology
* **Language:** Python
* **Recommendation Engines & Modeling:** `scikit-learn` (Cosine Similarity, Pairwise distances), `scipy.sparse` (Compressed Sparse Row matrices)
* **Data Processing:** `pandas` (Pivot tables, merging unstructured metadata, matrix reshaping), `numpy`
* **Visualization:** `seaborn`, `matplotlib` (Distribution curves, long-tail plots, correlation maps)

---

## 💻 How to Run This Project

### 1. Clone this repository
```bash
git clone https://github.com
cd zee-recommender-system
```

### 2. Install the required dependencies
Ensure your virtual environment is active, then install the packages:
```bash
pip install -r requirements.txt
```

### 3. Open the notebook
Launch the Jupyter ecosystem to explore user preferences and validation loops:
```bash
jupyter notebook Zee_Recommender_Systems.ipynb
```

