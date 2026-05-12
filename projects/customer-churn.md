---
layout: default
title: Customer Churn Prediction & Segmentation
permalink: /projects/customer-churn/
---

# Customer Churn Prediction & Segmentation
**Fitness Chain · Scikit-learn · K-Means · Logistic Regression**

[← Back to Projects](/projects/)

---

## Business Context

A gym chain needed to understand which customers were likely to cancel 
their membership and why. The goal was to move from reactive retention 
to a proactive, data-driven strategy based on behavioral profiles.

---

## Objectives

- Predict churn probability for each customer in the following month
- Identify the most influential features driving cancellations
- Segment customers into behavioral clusters
- Deliver cluster-specific retention recommendations

---

## Methodology

**1. Exploratory Data Analysis**
No missing values or duplicates found. Compared mean feature values 
between churned and retained customers. Key findings:
- Multicollinearity detected: Contract_period / Month_to_end_contract (r ≈ 0.97)
- Strongest negative correlations with churn: Lifetime (-0.44), 
Avg_class_frequency (-0.41), Age (-0.40)

**2. Churn Prediction Models**

| Model | Accuracy | Precision | Recall |
|---|---|---|---|
| Logistic Regression | 92% | 86% | 83% |
| Random Forest | 92% | Lower | Lower |

Logistic Regression selected as preferred model based on superior 
precision and recall for identifying at-risk customers.

**3. Customer Segmentation — K-Means (n=5)**
Data standardized prior to clustering. Dendrogram used to estimate 
optimal cluster count. Two high-risk clusters identified:
- **Cluster 2:** No customers live near a facility; low class frequency 
and low community engagement (churn ~51%)
- **Cluster 3:** Youngest group, shortest tenure, lowest class attendance 
and additional spending (churn ~44%)

---

## Key Findings

- Customers who churn tend to be younger, have short contracts, low 
class attendance, and weak social ties to the gym community
- Geographic distance from facilities is a critical churn factor 
independent of contract length
- Customers without a registered phone number show intermediate churn risk

---

## Recommendations

- **Cluster 2:** Promote group classes and referral programs; explore 
distance-based discounts to incentivize attendance
- **Cluster 3:** Incentivize longer contracts from sign-up; offer 
discounts on additional services to increase engagement
- **Acquisition:** Segment new customer promotions by geographic 
proximity to facilities

---

## Resources

- 📓 [View Notebook on GitHub](https://github.com/Esparza-Data-An/Customer-Retention-Analysis-Fitness-Chain)

---

[← Back to Projects](/projects/)