---
layout: default
title: Inefficient Operator Detection
permalink: /projects/operator-detection/
---

# Inefficient Operator Detection
**Virtual Telephony Platform · Python · SciPy · Tableau**

[← Back to Projects](/projects/)

---

## Business Context

A virtual telephony platform needed a reliable method to identify 
underperforming operators — not based on intuition, but on measurable, 
statistically validated evidence. The challenge: raw missed call rates 
were misleading because operators handle very different call volumes.

---

## Objectives

- Design an evidence-based scoring methodology to classify operator inefficiency
- Correct for dataset skewness caused by unequal call volumes
- Validate the scoring system through statistical hypothesis testing
- Deliver actionable recommendations for personnel review and technical auditing

---

## Methodology

**1. EDA & Data Cleaning**
Volume-weighted analysis using call count as a correction factor, 
revealing a true missed call rate above 50% — nearly 20 points higher 
than naive baseline estimates.

**2. Operator Metrics**
Five aggregated metrics derived per operator:
- Average wait time
- Incoming missed call rate
- Outbound missed call rate
- Total outbound volume
- Zero-duration call ratio (ghost call detection)

**3. Inefficiency Scoring**
Evidence-based thresholds assigned 1 point per rule violated. 
Operators scoring ≥ 3 classified as critically inefficient.

**4. Statistical Validation**
Three hypotheses tested using Mann-Whitney U and Spearman correlation 
(α = 0.05), confirming the scoring system's reliability and detecting 
a systematic ghost call pattern (ρ = 0.9996).

---

## Key Results

- **70 critically inefficient operators** identified (6.6% of total)
- **2 extreme cases** with outbound loss rates ≥ 83% and near-zero call duration
- Statistical validation confirmed significant separation between 
efficient and inefficient groups (p ≈ 0)

---

## Recommendations

- Priority review of all 70 flagged operators, with immediate focus 
on the 2 highest-scoring cases
- Technical audit of call routing to investigate ghost call patterns
- Role reassignment for operators with low outbound volume but 
outbound responsibilities
- Implementation of periodic monthly monitoring using this scoring pipeline

---

## Resources

- 📓 [View Notebook on GitHub](https://github.com/Esparza-Data-An/Operational-Efficiency-Analysis-Virtual-Telephony-Platform)
- 📊 [Interactive Dashboard on Tableau Public](https://public.tableau.com/views/Listadeoperadores-CallMeMaybe/Dashboard2)

---

[← Back to Projects](/projects/)