---
layout: default
title: Trip Duration Analysis
permalink: /projects/chicago-trips/
---

# Trip Duration Analysis
**Urban Mobility · SQL · Python · Statistical Testing**

[← Back to Projects](/projects/)

---

## Business Context

A Chicago cab service needed to understand whether external factors — 
specifically weather conditions — had a measurable impact on trip 
duration. The answer has direct implications for dynamic pricing, 
driver allocation, and demand forecasting.

---

## Objectives

- Extract and prepare data using SQL queries across multiple relational tables
- Analyze urban mobility patterns through EDA
- Test whether weather conditions significantly impact trip duration

---

## Methodology

**1. SQL Data Extraction**
Six queries designed to extract and prepare the data:
- Trip volume per taxi company
- Market share comparison between key competitors
- Weather classification per hour using CASE logic (Bad = rain/storm, Good = all others)
- Full trip records from Loop to O'Hare on Saturdays, joined with 
weather conditions and duration

**2. Exploratory Data Analysis**
- No missing values or type inconsistencies found
- Flash Cab identified as dominant company by trip volume
- Loop confirmed as the neighborhood with highest average trip completions

**3. Hypothesis Testing**
- **H₀:** Average trip duration does not change on rainy Saturdays
- **H₁:** Average trip duration changes on rainy Saturdays
- Test: Welch's t-test (selected due to significant difference in sample sizes)
- Significance level: α = 0.05

---

## Key Results

| Condition | Median Duration |
|---|---|
| Good Weather | 1,800s (30 min) |
| Bad Weather | 2,565s (42.75 min) |

- t-statistic: 7.478
- p-value: 1.11e-12 (≪ 0.05)
- **H₀ rejected.** Rain produces a systemic increase in trip duration

The difference in medians (12.7 min) exceeds the difference in means 
(7.2 min), indicating that rain shifts the entire distribution — 
increasing typical trip duration by over 20% on rainy Saturdays.

---

## Conclusions

Weather conditions have a statistically significant and practically 
meaningful impact on urban trip duration. Rain on Saturdays increases 
the typical Loop–O'Hare trip by nearly 13 minutes — a finding relevant 
for dynamic pricing, driver allocation, and demand forecasting models.

---

## Resources

- 📓 [View Notebook on GitHub](https://github.com/Esparza-Data-An/Mobility-Environmental-Impact-Study-Urban-Transportation-Service)

---

[← Back to Projects](/projects/)