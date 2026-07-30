<div align="center">

<!-- LOGO & TITLE SECTION -->
<br>
<img src="assets/AnalystAfrica_Logo.png" alt="AnalystLab Africa Logo" width="200">

<br><br>
# AnalystLab Africa — Data Science Internship

**Intern:** Thembinkosi Spogter Phama  
**Program:** 8-Week Data Science Internship  
**Duration:** 01 July 2026 - 01 September 2026

**Organization:** AnalystLab Africa  

<br>

[![Python](https://img.shields.io/badge/Python-3.14-blue?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-blue?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-orange?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org)

<br>

</div>

---

## 📁 Project Structure

![Project Structure](Week1-2_EDA/figures/dashboards/project_structure.png)

---

## 📋 Week-by-Week Progress

| Week | Topic | Status | Deliverables |
|------|-------|--------|--------------|
| **1–2** | Data Cleaning & EDA | ✅ Complete | Notebook, PDF Report, 11 Visuals, 2 Dashboards |
| 3 | Statistics & Probability | ✅ Complete | Statistical Analysis Report |
| 4 | Supervised Learning | 🔜 Upcoming | ML Models Notebook |
| 5 | Advanced ML | 🔜 Upcoming | Model Comparison Report |
| 6 | Feature Engineering | 🔜 Upcoming | Optimized Models |
| 7 | Model Deployment | 🔜 Upcoming | Flask/Streamlit App |
| 8 | Capstone Project | 🔜 Upcoming | End-to-End Project |

---

## ✅ Week 1–2: Data Cleaning & Exploratory Data Analysis

### 📊 Datasets Used

| Dataset | Rows | Columns | Source |
|---------|------|---------|--------|
| Titanic | 891 | 12 | Kaggle |
| Housing Prices | 545 | 13 | Kaggle |

### 🔧 Tasks Completed

- Loaded and explored both datasets
- Handled missing values (Age: median, Embarked: mode, Cabin: dropped)
- Removed duplicates
- Performed univariate & bivariate analysis
- Created **11 individual visualizations**
- Built **2 comprehensive dashboards**
- Generated correlation heatmaps
- Identified key predictors for modeling

### 💡 Key Insights

<details>
<summary><b>🚢 Titanic Dataset Insights (Click to expand)</b></summary>
<br>

- **Overall Survival Rate:** 38.4% (342 out of 891 passengers)
- **Gender Impact:** Women survived at a significantly higher rate (74.2%) than men (18.9%)
- **Class Impact:** 1st class (62.9%), 2nd class (47.3%), 3rd class (24.2%)
- **Age Pattern:** Most passengers aged 20–40; children had higher survival rates
- **Top Predictors:** Pclass (-0.34), Fare (+0.26)

</details>

<details>
<summary><b>🏠 Housing Dataset Insights (Click to expand)</b></summary>
<br>

- **Price Range:** 1.3M to 13.3M
- **Strongest Price Predictor:** Area (+0.54 correlation)
- **Furnishing Impact:** Furnished houses command premium prices
- **Top Predictors:** Area (0.54) → Bathrooms (0.52) → Stories (0.42) → Parking (0.38) → Bedrooms (0.37)

</details>

---

## 🛠️ Technologies Used

| Category | Tools |
|----------|-------|
| **Language** | Python 3.14 |
| **Data Manipulation** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **Notebook** | Jupyter Notebook |
| **Reports** | fpdf2 |
| **Version Control** | Git & GitHub |

---

## 📂 Week 1–2 Deliverables

- **Jupyter Notebook:** `Week1-2_EDA/Week1-2_EDA.ipynb`
- **PDF Report:** `Week1-2_EDA/Week1-2_EDA_Report.pdf`
- **Dashboards (2):** `Week1-2_EDA/figures/dashboards/`
  - Titanic Dashboard
  - Housing Dashboard
- **Visuals (11):** `Week1-2_EDA/figures/visuals/`
  - Titanic (6 visualizations)
  - Housing (5 visualizations)
- **Cleaned Datasets:** `datasets/`
  - titanic_cleaned.csv
  - housing_cleaned.csv

---
## ✅ Week 3: Statistics & Probability

### Topics Covered

- Descriptive Statistics (mean, variance, skewness, kurtosis)
- Probability Distributions (Normal, Right-Skewed)
- Hypothesis Testing (T-Test, Chi-Square)
- Correlation vs Causation

### Hypothesis Testing Results (Alpha = 0.05)

| # | Test | Type | p-value | Result |
|---|------|------|---------|--------|
| 1 | Age: Survivors vs Non-Survivors | T-Test | 0.0528 | ❌ NOT Significant |
| 2 | Fare: 1st Class vs 3rd Class | T-Test | < 0.001 | ✅ HIGHLY Significant |
| 3 | Survival vs Gender | Chi-Square | < 0.001 | ✅ HIGHLY Significant |
| 4 | Price: AC vs No AC (Housing) | T-Test | < 0.001 | ✅ HIGHLY Significant |

### Key Insights

<details>
<summary><b>📊 Statistical Findings (Click to expand)</b></summary>
<br>

- **Age** is near-normally distributed (skew=0.51, mean≈median)
- **Fare** is heavily right-skewed (skew=4.79) with mean (32.2) >> median (14.5)
- **Housing Price & Area** are moderately right-skewed (skew ~1.2-1.3)
- **Gender** is the most significant survival predictor (Chi-Square = 260.7)
- **Air Conditioning** adds significant value to houses (~1.8M difference)

</details>

<details>
<summary><b>⚠️ Correlation ≠ Causation (Click to expand)</b></summary>
<br>

- **Fare & Survival (r=0.26):** Fare is a proxy for Class, not a direct cause
- **Bedrooms & Price (r=0.37):** Area (r=0.54) is the real driver
- **Age & Survival (r=-0.06):** Not even statistically significant (p=0.0528)

</details>

---

## 📂 Week 3 Deliverables

- **Jupyter Notebook:** `Week3_Statistics/Week3_Statistics.ipynb`
- **PDF Report:** `Week3_Statistics/Week3_Statistics_Report.pdf`
- **Dashboards (2):** `Week3_Statistics/figures/dashboards/`
  - Titanic Statistical Dashboard
  - Housing Statistical Dashboard
- **Visuals (4):** `Week3_Statistics/figures/visuals/`
  - Distribution Comparison
  - Hypothesis Test Results
  - Titanic Correlation Heatmap
  - Housing Correlation Heatmap
    
## 🔗 Connect

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=for-the-badge&logo=github)](https://github.com/)

<br>

### Made with dedication during the AnalystLab Africa Internship Program

**#AnalystLabAfrica #DataScience #EDA #Python #MachineLearning #DataAnalytics**

</div>
