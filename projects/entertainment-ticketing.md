---
layout: default
title: Data-Driven Growth Analytics: Optimizing User Cohorts and Marketing ROI
permalink: /projects/marketing-growth-ticketing/
---

# Data-Driven Growth Analytics: Optimizing User Cohorts and Marketing ROI
**Growth Analytics · Multichannel ROI · Cohort Analysis · Python · Power BI**

[← Back to Projects](/projects/)

---

## Business Context

An entertainment ticketing platform required a comprehensive diagnostic of its user behavior and marketing spend efficiency. The operation needed to understand purchase velocity, identify high-value customer segments, and evaluate the true return on its advertising investments across multiple acquisition channels.

---

## Objectives

- Profile platform engagement (DAU, WAU, MAU) and diagnose retention barriers.
- Segment buyers into conversion cohorts to measure purchase velocity, Customer Lifetime Value (LTV), and average ticket.
- Quantify Customer Acquisition Cost (CAC) and Return on Marketing Investment (ROMI) across 7 channels to reallocate budget efficiently.

---

## Methodology

**1. Data Pipeline & Feature Engineering**
- Standardized cross-dataset headers to `lower_snake_case` and cast timestamps to `datetime64[ns]`.
- Engineered explicit session durations and built purchase-velocity cohorts using first-visit and first-purchase timestamps.
- Applied **volume‑weighted aggregation** (by `calls_count`) to correct for dataset skewness during exploratory analysis.

**2. Product Dynamics & Seasonality**
- Established traffic baselines: **DAU (908 unique users)** and **WAU (5,716 unique users)**.
- Detected strong late‑Q4 cyclical peaks (November Black Friday) and a retention bottleneck: only **19.7%** of users return on distinct days.
- Identified **intensive single‑day users** (multiple sessions on the same day but no return) with a purchase rate of **40.60%** vs. **10.47%** for single‑session users (Z‑test, p=0).

**3. Cohort & Marketing Performance Optimization**
- Segmented buyers into conversion‑velocity windows (C0, C1, C2‑7, C8‑30, C30+).
- Used **first‑touch attribution** to assign revenue to the marketing source that originally acquired the user, avoiding revenue inflation from multiple sessions.
- Mapped transactional revenue against daily ad spend to calculate unit CAC and channel‑specific ROMI.

---

## Key Results

### User Cohort Architecture

| Cohort Window | % Share | Avg. Ticket | User LTV | Key Takeaway |
| :--- | :---: | :---: | :---: | :--- |
| **C0 (Immediate / Day 0)** | 72.2% | $4.56 | $5.92 | Core volume driver but lowest individual LTV. |
| **C1 (1 Day)** | 2.8% | $5.90 | $10.57 | Small but high‑ticket segment. |
| **C2‑7 (2 to 7 Days)** | 5.7% | $4.79 | $7.99 | Moderate value, short research phase. |
| **C8‑30 (8 to 30 Days)** | 6.0% | $7.82 | $13.47 | Highest transactional health; intensive research phase. |
| **C30+ (Over 30 Days)** | 13.4% | $5.50 | $8.04 | Late buyers with intermediate LTV. |

**Insight:** C8‑30 users represent only 6% of buyers but generate the highest LTV ($13.47) and average ticket ($7.82), making them the prime target for retargeting and nurturing campaigns.

### Multichannel Acquisition Efficiency

| Source ID | Total Spend | Unit CAC | Attributed Revenue | ROMI (%) | Operational Action |
| :---: | :---: | :---: | :---: | :---: | :--- |
| **1** | $20,833.27 | $1.10 | $2,298,200.17 | **10,931.4%** | Highly Recommended (High Efficiency) |
| **2** | $42,806.04 | $1.63 | $2,638,189.21 | **6,063.1%** | Highly Recommended (Maximum Scale) |
| **3** | $141,321.63 | $1.89 | $296,687.96 | **109.9%** | Weak Performance (Highly Inefficient) |

* **Structural Inefficiency:** Source 3 commanded the highest budget allocation ($141.3K) while operating at a near‑break‑even **109.9% ROMI**, severely dragging down corporate margins.

### Quality of Traffic (Integrated View)

| Source | ROMI | CAC | % No Buyers | % C0 | % C8‑30 | Avg. Days Active | Avg. Session Duration |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| 1 | 49% | $2.20 | 69% | 24% | 2% | 2.08 | 12.18 min |
| 3 | -61% | $2.14 | 84% | 11% | 1% | 1.41 | 8.89 min |
| 9 | 4% | $0.86 | 83% | 8% | 2% | 1.82 | 8.74 min |

**Key Takeaways:**
- **Source 1** is the most efficient channel (ROMI 49%) with the highest retention (2.08 days) and session duration (12.18 min).
- **Source 3** is inefficient (−61% ROMI) due to low‑quality traffic (84% non‑buyers, low retention).
- **Source 9** shows a distinct late‑buyer profile (6% C30+) and deserves monitoring.

---

## Conclusions

To optimize commercial growth, capital must be **immediately reallocated** from Source 3 toward high‑efficiency scaling channels (Sources 1, 2, and 5). Additionally:
- Integrate **upselling and cross‑selling** mechanisms into the immediate C0 funnel to expand their low average ticket.
- Deploy **targeted retargeting campaigns** for the high‑value C8‑30 mid‑funnel segment.
- Monitor Source 9 as a potential long‑term cultivation channel.

---

## Interactive Dashboard

A Power BI dashboard was built to allow stakeholders to explore these insights interactively. It includes three pages:
1. **Executive Summary** – Global KPIs, LTV by cohort, and ROMI by channel.
2. **Marketing Efficiency** – CAC/ROMI comparison per channel with detailed traffic quality metrics.
3. **Cohort Analysis** – LTV, average ticket, and orders per user, with an interactive filter by device (`desktop` / `touch`).

### Dashboard Preview
![Executive Summary](images/dashboard_page1.png)
![Marketing Efficiency](images/dashboard_page2.png)
![Cohort Analysis](images/dashboard_page3.png)

📊 [Download the .pbix file](https://github.com/Esparza-Data-An/Data-Driven-Growth-Analytics--Optimizing-User-Cohorts-and-Marketing-ROI-for-Entertainment-Ticketing/blob/main/growth_analytics_dashboard.pbix) *(requires Power BI Desktop)*

---

## Resources

- 📓 [View Notebook on GitHub](https://github.com/Esparza-Data-An/Data-Driven-Growth-Analytics--Optimizing-User-Cohorts-and-Marketing-ROI-for-Entertainment-Ticketing)


[← Back to Projects](/projects/)