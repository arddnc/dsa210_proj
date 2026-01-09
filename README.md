# 🏈 Is Tom Brady Really the GOAT?
*A Data-Driven Comparison of NFL Quarterbacks*

---

## 👤 Student Information
- **Name:** Arda Dinç  
- **Course:** DSA210 – Introduction to Data Science (Fall 2025)

---

## 🎯 Motivation

Tom Brady is widely regarded as the greatest quarterback of all time (GOAT), but this claim is often based on subjective arguments such as championships and popularity.  
This project aims to evaluate Brady’s GOAT status from a **data-driven perspective**, using statistical analysis and machine learning techniques.

By comparing Tom Brady’s season-level performance with other elite quarterbacks (Peyton Manning, Aaron Rodgers, Patrick Mahomes, and Joe Montana), the project investigates whether Brady’s legacy is supported by measurable performance indicators.

---

## 📦 Data Sources

Season-level quarterback statistics were collected from **Pro-Football-Reference (PFR)** player pages:

- Tom Brady – https://www.pro-football-reference.com/players/B/BradTo00.htm  
- Peyton Manning – https://www.pro-football-reference.com/players/M/MannPe00.htm  
- Aaron Rodgers – https://www.pro-football-reference.com/players/R/RodgAa00.htm  
- Patrick Mahomes – https://www.pro-football-reference.com/players/M/MahoPa00.htm  
- Joe Montana – https://www.pro-football-reference.com/players/M/MontJo01.htm  

The tables were imported using `pandas.read_html()` and combined into a single dataset.

**Main features used in the analysis:**
- Season (Year)
- Games played (G)
- Passing yards (Yds)
- Touchdowns (TD)
- Interceptions (Int)
- Passer rating (Rate)
- Player name

---

## 🔬 Data Analysis

### Data Cleaning & Feature Engineering
The collected data was cleaned by standardizing column names, converting numeric fields, and handling missing values.  
Additional features were derived to support the analysis, including:
- **TD/INT ratio** (passing efficiency)
- **Yards per game**

Each row in the final dataset represents a single quarterback season.

---

### 📊 Exploratory Data Analysis (EDA)
EDA was conducted using visualizations such as line plots and boxplots to compare:
- Passing efficiency across seasons
- Distribution of performance metrics among quarterbacks
- Differences between Brady and his peers

---

### 🧪 Hypothesis Testing
A two-sample t-test was performed to evaluate whether Tom Brady’s season-level passing efficiency (TD/INT ratio) is statistically different from that of other elite quarterbacks.

The results showed **no statistically significant difference**, suggesting that Brady’s advantage does not primarily come from superior single-season efficiency.

---

## 🤖 Machine Learning Analysis

A **logistic regression** model was trained to classify whether a quarterback season is **elite**, defined as being in the top 25% of passer rating across all seasons.

- **Model accuracy:** 0.88

When the trained model was applied to Tom Brady’s seasons:
- **3 out of 23 seasons** were classified as elite (≈13%)

This indicates that while Brady does not consistently dominate efficiency metrics, his legacy is better explained by **long-term consistency and career longevity** rather than frequent peak seasons.

---

## 📌 Findings

- Tom Brady’s per-season efficiency is not significantly higher than other elite quarterbacks.
- Brady’s distinguishing factor is sustained high-level performance across many seasons.
- Machine learning results support the interpretation that longevity and consistency play a central role in Brady’s GOAT status.

---

## ⚠️ Limitations & Future Work

- The analysis focuses on regular-season statistics and does not include postseason performance.
- Contextual factors such as team strength and coaching are not explicitly modeled.
- Future work may incorporate playoff data and alternative machine learning models to further explore quarterback greatness.
