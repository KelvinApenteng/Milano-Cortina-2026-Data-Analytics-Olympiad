# 🏅 Milano Cortina 2026 Winter Olympics Data Analytics Olympiad  
## USA vs Canada: Who Really Outperformed Expectations?

---

# Introduction

Welcome to our full submission for the **Data Analytics Olympiad 2026**, where teams were challenged to solve a real-world sports analytics case using athlete-level data from the **Milano Cortina 2026 Winter Olympics**.

This project combined:

- Data Cleaning  
- Exploratory Data Analysis  
- Predictive Machine Learning  
- Executive Strategy Reporting  

The challenge required teams to move beyond simple statistics and develop a complete analytical story around Olympic performance, medal efficiency, and future investment strategy.

---

# Core Challenge Question

> Did the United States truly outperform Canada at Milano Cortina 2026, or did another nation generate greater value relative to its resources?

This question was explored through four major tasks:

1. Data Cleaning & Preprocessing  
2. Exploratory Data Analysis & Storytelling  
3. Predictive Modeling  
4. Business Insight Report & Strategic Recommendations  

---

# Team Members

### Team 1 – Canisius University

- Apenteng Kelvin Cecil  
- Crooks Andrew  
- Baddley Micheal  
- Hasnat Sayed Abu  

---

# Project Objectives

The primary objectives of this Olympiad project were to:

- Prepare a high-quality Olympic athlete dataset for analysis  
- Compare USA and Canada athlete systems using evidence  
- Identify medal-winning athlete characteristics  
- Build machine learning models to predict medal success  
- Translate analytics into executive recommendations for 2030 Olympic planning  

---

# Dataset Overview

The project used a Winter Olympics athlete dataset containing competitors from multiple nations and sports disciplines.

### Original Dataset:

| Metric  | Value |
|---------|------|
| Rows    | 390 |
| Columns | 17 |
| Nations | Multiple |
| Sports  | Multiple Winter Sports |

### Final Cleaned Dataset:

| Metric              | Value |
|---------------------|-------|
| Rows                | 387   |
| Columns             | 23    |
| Missing Values      | 0     |
| Engineered Features | 6     |

---

# Task 1 — Data Cleaning and Preprocessing

The first stage focused on transforming messy raw data into an analysis-ready dataset.

## Key Cleaning Actions

### Missing Value Treatment

Variables such as:

- VO2max  
- Body_Fat_Pct  
- Training_Hours_Per_Week  
- Altitude_Training_m  

were imputed using **sport-specific median values**.

### Impossible Values Corrected

Examples detected:

- Age = 9  
- VO2max = -8.4  
- Training Hours = 172  
- Body Fat = 99.2  

These were corrected using structured imputation.

### Duplicate Detection

Three hidden duplicate athlete records were removed.

## Feature Engineering

New variables created:

- Medal_Won  
- Experience_Index  
- VO2_BodyFat_Ratio  
- GDP_Tradition_Score  
- Reaction_Time_Missing  
- WorldCupPoints_Missing  

## Key Outcome

A robust analytical dataset suitable for modeling, visualization, and strategy development.

---

# Task 2 — Exploratory Data Analysis & Storytelling

Task 2 answered six Olympic performance questions using charts, comparative statistics, and written interpretation.

---

## USA vs Canada Findings

### USA Won Through:

- Broader medal pathways  
- Greater sport diversification  
- Higher gold medal conversion  
- Strong physiological outliers  
- Better use of broad system depth

### Canada Competed Through:

- Winter sport tradition  
- Strong performances in key sports  
- Veteran athlete strength  
- Focused excellence in selected disciplines

---

## Key EDA Insights

### 1. Sport Portfolio Matters

The USA succeeded across more sports, reducing medal risk concentration.

Canada’s success was more dependent on:

- Speed Skating  
- Curling  
- Hockey  
- Short Track  

### 2. Gold Medalists Shared Common Traits

Gold medal winners generally showed:

- Higher VO2max  
- Higher training volume  
- Prime competitive age  
- Prior Olympic experience

### 3. Peak Performance Window

Most medal success occurred between ages:

**29–36**

Though sport-specific variation existed.

### 4. GDP Helps, But Strategy Wins

Norway’s dominance showed that targeted systems and winter sport identity may outperform economic scale alone.

---

# Task 3 — Predictive Modeling

Machine learning models were built to predict whether an athlete would win:

## Medal vs No Medal

(Binary Classification)

---

# Models Developed

### 1. Logistic Regression  
### 2. Random Forest Classifier

---

# Final Best Model: Logistic Regression

| Metric    | Score |
|-----------|-------|
| Accuracy  | 82.1% |
| Precision | 64.0% |
| Recall    | 76.2% |
| F1 Score  | 69.6% |
| AUC ROC   | 84.4% |

---

# Why Accuracy Alone Was Not Enough

Because only **26.9%** of athletes won medals.

A model predicting “No Medal” for everyone could still appear accurate.

Therefore we emphasized:

- Recall  
- Precision  
- F1 Score  
- ROC-AUC

---

# Top Predictors of Medal Success

Our model found the strongest medal indicators were:

- High VO2max  
- Strong training volume  
- Previous Olympic appearances  
- Low injury burden  
- Strong national systems  
- Participation in medal-efficient sports

---

# USA vs Canada Athlete Prediction Test

The final model was tested on seven real athletes:

| Athlete               | Country | Prediction|
|-----------------------|---------|-----------|
| Mikaela Shiffrin      | USA     | Medal     |
| Jordan Stolz          | USA     | Medal     |
| Elana Meyers Taylor   | USA     | Medal     |
| Courtney Sarault      | CAN     | Medal     |
| Metodej Jilek         | CZE     | Medal     |
| Deanna Stellato-Dudek | CAN     | Medal     |
| Connor McDavid        | CAN     | No Medal  |

---

# Strategic Insight from Modeling

The USA showed stronger medal depth probabilities.

Canada remained highly dangerous in:

- Short Track  
- Figure Skating  
- Hockey  
- Sliding Sports

---

# Task 4 — Executive Strategic Report

Prepared for:

- United States Olympic & Paralympic Committee (USOPC)  
- Canada’s Own the Podium Program  

---

# Objective

Recommend how to allocate:

## $200 Million in Olympic development funding before the **2030 French Alps Winter Olympics**.

---

# Recommended Funding Strategy

| Nation | Allocation |
|--------|------------|
| USA    | $110M      |
| Canada | $90M       |

---

# USA Recommendations

- Protect Alpine Skiing pipelines  
- Continue Bobsleigh investment  
- Expand Freestyle Skiing depth  
- Accelerate young Speed Skating talent

---

# Canada Recommendations

- Improve gold medal conversion systems  
- Focus on Short Track & Figure Skating  
- Expand Sliding Sports investment  
- Build next-generation athlete pipeline

---

# Projected Medal Uplift by 2030

| Nation | Gain            |
|--------|-----------------|
| USA    | +2 to +4 medals |
| Canada | +3 to +5 medals |

---

# Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- Jupyter Notebook  
- Microsoft Word  
- GitHub  

---

# Repository Structure

```text
Milano-Cortina-2026-Data-Analytics-Olympiad/
│── README.md
│── Task 1 Report.docx
│── Task 2 Report.docx
│── Task 3 Report.docx
│── Executive Strategic Report.docx
│── notebooks/
│── images/
│── data/