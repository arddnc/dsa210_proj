# 🏈 Is Tom Brady Really the GOAT?  
*A Data-Driven Comparison of NFL Quarterbacks*

---

## 👤 Student Information
- **Name:** Arda Dinç  
- **Course:** DSA210 – Introduction to Data Science (Fall 2025)   

---

## 🎯 Motivation

As someone who recently started following the NFL, I constantly hear that *“Tom Brady is the GOAT.”*  
But is he really?

This project aims to investigate that question by using the data analysis and statistical techniques I’ve learned in class.  
I will compare Tom Brady’s career performance statistics with other elite quarterbacks (such as Peyton Manning, Aaron Rodgers, and Patrick Mahomes) to evaluate whether Brady’s legendary status is truly supported by the data.

The main goal is to move beyond opinions and use objective analysis to explore what really makes someone the **Greatest of All Time**.

---

## 📦 Data Sources

1. **NFL Player Career Statistics (Primary Dataset)**  
   - **Source:** [Pro-Football-Reference](https://www.pro-football-reference.com/players/)  
   - **Access:** Publicly available tables that can be downloaded as CSV or collected via `pandas.read_html()` in Python.  
   - **Players to Compare:**  
     - Tom Brady  
     - Peyton Manning  
     - Aaron Rodgers  
     - Patrick Mahomes  
     - Joe Montana  
   - **Main Features:** Season, Team, Games, Passing Yards, Touchdowns (TD), Interceptions (INT), Completion %, QBR, Wins, and Super Bowl results.

2. **Enrichment**  
   - Awards or team performance data from the same site (e.g., MVP, All-Pro selections, win percentages).  
   - This can provide an additional layer of context for comparing recognition and consistency.

---

## 🔬 Analysis Plan

### 1️⃣ Data Collection & Cleaning
Career data for each quarterback (Tom Brady, Peyton Manning, Aaron Rodgers, Patrick Mahomes, etc.) will be gathered from [Pro-Football-Reference](https://www.pro-football-reference.com/players/).  
All tables will be combined into a single dataset using Python (`pandas`).  
Column names will be standardized, datatypes unified, and missing values handled to ensure comparability.  
This stage will produce a clean DataFrame where each row represents a player–season record.

---

### 🧩 2️⃣ Feature Engineering
To enhance interpretability and fairness of comparisons, several new metrics will be derived from the raw statistics.  
These engineered features will measure not only total production but also efficiency and consistency across seasons.

**Planned engineered features:**

- **TD/INT Ratio:**  
  Touchdowns divided by interceptions — measures passing efficiency and decision-making quality (how productive and error-free a quarterback is).

- **Yards per Game:**  
  Total passing yards divided by games played — normalizes for players who played different numbers of games, allowing fairer comparisons.

- **Win Percentage:**  
  Total team wins divided by games played — represents the quarterback’s contribution to overall team success beyond individual performance.

- **Career Averages and Standard Deviations:**  
  Average and variability of core metrics (yards, TD, QBR) across seasons — evaluates long-term stability rather than single-season peaks.

Together, these engineered features will provide a stronger analytical foundation for hypothesis testing and visualization, enabling a more data-driven evaluation of whether Tom Brady’s performance truly supports his GOAT status.

---

### 📊 3️⃣ Exploratory Data Analysis (EDA)
Visualizations such as line charts, boxplots, and heatmaps will be used to explore differences among players.  
Example analyses include:  
- Year-over-year trends of passing yards, touchdowns, and interceptions.  
- Distribution comparisons of TD/INT ratio and QBR.  
- Correlation heatmaps to understand relationships among metrics.

---

### 🧪 4️⃣ Hypothesis Testing
To statistically assess whether Tom Brady’s performance is superior to his peers:

- **Null Hypothesis (H₀):** Brady’s performance metrics are not significantly different from other elite quarterbacks.  
- **Alternative Hypothesis (H₁):** Brady’s performance metrics are significantly higher than his peers.  

Two-sample t-tests or ANOVA will be used depending on data structure.  
Results will indicate whether observed differences are statistically significant.

---

### 📈 5️⃣ Visualization Plan
Key visualizations will summarize and compare player performance:

- **Line Charts:** Season-by-season passing yards and touchdowns.  
- **Bar Charts:** Average QBR, TD/INT ratio, and win percentage per player.  
- **Heatmap:** Correlation among all metrics to highlight efficiency and stability patterns.  

These visuals will support clear communication of the results and provide intuitive evidence for or against the “Brady = GOAT” hypothesis.

---

## 📊 Expected Findings

Based on existing discussions and early data exploration, the analysis is expected to reveal the following insights:

- **Career Consistency:**  
  Tom Brady is anticipated to outperform other quarterbacks in terms of long-term stability.  
  His ability to maintain high-level performance over two decades is likely to result in lower variability (standard deviation) across metrics such as passing yards and TD/INT ratio.

- **Peak Efficiency Comparison:**  
  Quarterbacks like **Patrick Mahomes** or **Peyton Manning** may demonstrate higher short-term efficiency — achieving superior QBR or TD/INT ratios during their prime seasons.  
  This would show that Brady’s greatness is not purely about peak dominance but about sustained excellence.

- **Team Impact:**  
  Brady’s win percentage is expected to remain among the highest, reinforcing his influence on overall team success.  
  This metric may serve as a bridge between individual performance and collective outcomes.

- **GOAT Interpretation:**  
  The data will likely support that “being the GOAT” involves a combination of **longevity, consistency, and championship impact**, rather than single-season dominance.  
  The project aims to quantify how Brady balances these factors compared to his peers.

Ultimately, the findings will help clarify whether Tom Brady’s legendary reputation is statistically justified — or if the GOAT debate remains more subjective than data-driven.

---

## ⚙️ Tools & Environment

| Category | Tools / Libraries |
|-----------|-------------------|
| **Programming Language** | Python |
| **Data Handling** | pandas, numpy |
| **Visualization** | matplotlib, seaborn |
| **Statistical Analysis** | scipy.stats |
| **Environment** | Jupyter Notebook / Google Colab |
| **Version Control** | GitHub (for project submission and README) |
