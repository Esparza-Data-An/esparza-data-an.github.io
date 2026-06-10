---
layout: default
title: User Behavior Analysis & A/A/B Test
permalink: /projects/foodtech-ab-testing/
---

# User Behavior Analysis & A/A/B Testing in Food Tech
**Product Analytics · Conversion Funnels · Hypothesis Testing · A/A/B Experiments**

[← Back to Projects](/projects/)

---

## Business Context

A food products startup wanted to investigate user behavior across its mobile application. The company was facing two distinct challenges: identifying where potential customers drop off within the purchasing pipeline and evaluating whether a proposed typography/font change would statistically improve or hinder user conversion rates.

---

## Objectives

- Reconstruct and analyze the behavioral sales funnel to pinpoint the primary user bottleneck.
- Validate the integrity of the experimental setup through an A/A control group check.
- Execute multi-group hypothesis testing (A/A/B) to assess the impact of the new interface design.

---

## Methodology

**1. Data Cleansing & Validation**
- Filtered out log anomalies and incomplete tracking segments, safely removing ~3,000 records prior to 2019-08-01 to preserve analytical integrity.
- Verified homogeneous user distribution across control groups (246/247) and the active font-test group (248).

**2. Funnel Reconstruction**
- Mapped user journeys across sequential stages (`MainScreen` → `OffersScreen` → `CartScreen` → `PaymentSuccessful`), excluding non-sequential interactions like tutorials.

**3. Statistical Experimentation**
- Performed Z-tests for proportions across all stages to validate control consistency (A/A) and measure design changes (A vs. B).
- Implemented a **Bonferroni correction** threshold ($\alpha = 0.003125$) across 16 simultaneous comparisons to prevent Type I error inflation.

---

## Key Results

### Sales Funnel Dynamics
- **45.51%** of unique users complete the full journey from the initial application touchpoint to a successful payment.
- **The Core Bottleneck:** The largest drop-off occurs immediately at the **MainScreen → OffersScreen** transition, where **38.09% of users are lost**.

'''text
[Main Screen: 7,419 Users]  ──(100%)
      ↓
[Offers Screen: 4,593 Users] ──(60.96% Overall / 39.04% Drop-off)
      ↓
[Cart Screen: 3,734 Users]   ──(49.56% Overall / 18.70% Drop-off)
      ↓
[Successful Pay: 3,539 Users]──(46.97% Overall / 5.22% Drop-off)
'''

### Experimental Outcomes
- **A/A Validation Check:** Confirmed no statistically significant differences between control groups 246 and 247 ($p > 0.05$), proving the randomization algorithm worked perfectly.
- **A/A/B Evaluation:** Z-tests revealed no statistically significant impact on conversion metrics at any stage of the funnel under the font modification condition ($p > 0.05$), even under strict Bonferroni adjustments.

---

## Conclusions

The proposed typography change does not yield a statistically significant impact on conversion behavior. The data suggests retaining the original font configuration. Product optimization efforts should pivot away from cosmetic interface tweaks and focus on resolving the structural 38% user drop-off observed at the first transition of the funnel.

---

## Resources

- 📓 [View Notebook on GitHub](https://github.com/Esparza-Data-An/User-Behavior-Analysis---A-A-B-Test---Food-Tech-App)

---

[← Back to Projects](/projects/)