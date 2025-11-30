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

### 1. **NFL Player Career Statistics (Primary Dataset)**  
Career performance data for each quarterback will be collected from individual Pro-Football-Reference (PFR) player pages:

- **Tom Brady:** https://www.pro-football-reference.com/players/B/BradTo00.htm  
- **Peyton Manning:** https://www.pro-football-reference.com/players/M/MannPe00.htm  
- **Aaron Rodgers:** https://www.pro-football-reference.com/players/R/RodgAa00.htm  
- **Patrick Mahomes:** https://www.pro-football-reference.com/players/M/MahoPa00.htm  
- **Joe Montana:** https://www.pro-football-reference.com/players/M/MontJo01.htm  

These pages include structured statistical tables (passing, advanced metrics, season summaries) that can be directly imported using  
`pandas.read_html()` in Python.

**Main Features Collected:** Season, Team, Games, Passing Yards, Touchdowns (TD), Interceptions (INT), Completion %, QBR, Wins, and Super Bowl results.

---

### 2. **Enrichment Dataset**  
Additional data will be collected to provide context on awards and team success:

- **NFL Awards (MVP, All-Pro selections, etc.):**  
  https://www.pro-football-reference.com/awards/

- **NFL Team Standings & Win Percentages (by year):**  
  https://www.pro-football-reference.com/years/

These datasets will help evaluate recognition, consistency, and team performance alongside individual statistics.
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

### 🧪 Hypotheses

To rigorously evaluate whether Tom Brady deserves the GOAT title, multiple hypotheses will be tested:

- **H1: Efficiency Advantage**  
  Tom Brady’s TD/INT ratio is significantly higher than other elite quarterbacks.

- **H2: Consistency Advantage**  
  Tom Brady exhibits significantly lower year-to-year variability in key metrics (yards, TD, QBR).

- **H3: Longevity Effect**  
  Brady’s performance decline with age is significantly slower compared to peers.

- **H4: Game Impact Hypothesis**  
  Brady’s win percentage is significantly higher than other elite quarterbacks.

- **H5: Peak Performance Comparison**  
  There is no significant difference between Brady’s peak season and the peak seasons of Mahomes/Manning/Rodgers.

These hypotheses will be tested using statistical methods such as two-sample t-tests and ANOVA, depending on data structure.

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
