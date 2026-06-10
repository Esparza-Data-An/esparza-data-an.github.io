---
layout: default
title: Data-Driven Growth Analytics
permalink: /projects/marketing-growth-ticketing/
---

# Data-Driven Growth Analytics: Optimizing User Cohorts and Marketing ROI
**Growth Analytics · Multichannel ROI · Cohort Analysis · Python**

[← Back to Projects](/projects/)

---

## Business Context

An entertainment ticketing platform needed to map its user interaction profiles and evaluate its marketing spend architecture. The operation required a dual-stream diagnostic: uncovering friction points in the conversion funnel and isolating specific inefficiencies in digital acquisition channels to maximize Return on Marketing Investment (ROMI).

---

## Objectives

- Profile platform traffic dynamics (DAU, WAU, MAU) and identify retention barriers.
- Build time-based user cohorts to measure purchase velocity and Customer Lifetime Value (LTV).
- Quantify Customer Acquisition Cost (CAC) and ROMI across 7 marketing channels to optimize budget allocation.

---

## Methodology

**1. Data Pipeline & Feature Engineering**
- Standardized cross-dataset headers to `lower_snake_case` and recast object timestamps into explicit `datetime64[ns]` formats.
- Calculated explicit session durations and engineered discrete time-lag flags to isolate conversion velocity windows.

**2. Product Dynamics & Seasonality**
- Established traffic baselines: **DAU (908 unique users)** and **WAU (5,716 unique users)**, identifying strong late-Q4 cyclical spikes (November peak) and sharp contractions in August and April.
- Detected a retention bottleneck: returning users account for only **22.8%** of the total active user base.

**3. Cohort & Marketing Performance Optimization**
- Segmented buyers into conversion velocity windows (from Day 0 immediate purchase to 30+ days delays) to measure financial weight.
- Mapped cross-dataset transactional parameters against daily ad spend statistics to calculate unit CAC and channel-specific ROMI tiers.

---

## Key Results

### User Cohort Architecture

| Cohort Window | % Share | Avg. Ticket | User LTV | Key Takeaway |
| :--- | :---: | :---: | :---: | :--- |
| **C0 (Immediate / Day 0)** | 72.2% | $4.56 | $5.92 | Core volume driver but lowest individual LTV. |
| **C8-30 (8 to 30 Days)** | 6.0% | $7.82 | $13.47 | Highest transactional health; intensive research phase. |

### Multichannel Acquisition Efficiency

| Source ID | Total Spend | Unit CAC | Attributed Revenue | ROMI (%) | Operational Action |
| :---: | :---: | :---: | :---: | :---: | :--- |
| **1** | $20,833.27 | $1.10 | $2,298,200.17 | **10,931.4%** | Highly Recommended (High Efficiency) |
| **2** | $42,806.04 | $1.63 | $2,638,189.21 | **6,063.1%** | Highly Recommended (Maximum Scale) |
| **3** | $141,321.63 | $1.89 | $296,687.96 | **109.9%** | Weak Performance (Highly Inefficient) |

* **Structural Spend Inefficiency:** Source 3 commanded the highest budget allocation ($141.3K) while operating at a near-break-even **109.9% ROMI**, severely dragging down corporate margins.

---

## Conclusions

To optimize commercial growth, capital must be immediate reallocated from **Source 3** toward high-efficiency scaling channels (**Sources 1, 2, and 5**). Furthermore, cross-selling mechanisms must be integrated into the immediate `C0` funnel to expand their low average ticket, paired with targeted retargeting campaigns for the high-value `C8-30` mid-funnel segment.

---

## Resources

- 📓 [View Notebook on GitHub](https://github.com/Esparza-Data-An/Data-Driven-Growth-Analytics--Optimizing-User-Cohorts-and-Marketing-ROI-for-Entertainment-Ticketing)

---

[← Back to Projects](/projects/)