---
layout: default
title: Market & User Behavior Analysis
permalink: /projects/videogame-market/
---

# Market & User Behavior Analysis
**Global E-commerce (Gaming) · Python · SciPy · Seaborn**

[← Back to Projects](/projects/)

---

## Business Context

An online retailer operating worldwide needed to identify which platforms, 
genres, and regions represented the best opportunities for acquisition 
and advertising investment in 2017, based on historical sales patterns.

---

## Objectives

- Identify patterns determining commercial success across platforms and genres
- Build regional user profiles to support differentiated strategies
- Validate key assumptions through statistical hypothesis testing

---

## Methodology

**1. Data Preparation**
- Standardized column names and corrected data types
- Missing scores and TBD values converted to NaN
- ESRB ratings: missing values assigned to new unrated category
- Critic and user scores normalized to a unified 100-point scale
- Data filtered from 2005 onward to capture a full console generation cycle

**2. Exploratory Data Analysis**
- Peak release years: 2008–2009, declining post-2012
- Console lifecycle: ~10 years, with sales peaking ~5 years after launch
- Critic score correlation with sales: low-moderate (r ≈ 0.4)
- User score correlation with sales: near zero (r ≈ 0.1)
- Top genres by average sales: Shooter, Platform, Sports, Racing, Role-Playing

**3. Regional User Profiles**

| Region | Top Platforms | Top Genres | Notes |
|---|---|---|---|
| North America | X360, Wii, PS3 | Action, Sports, Shooter | PS4 gaining ground |
| Europe | PS3, X360, Wii | Action, Sports, Shooter | Racing genre appears |
| Japan | DS, 3DS, PS3 | Role-Playing, Action | Portable consoles dominant |

**4. Hypothesis Testing**
- **H1:** Xbox One vs. PC user ratings — H₀ rejected (p = 0.0037). 
Platforms should not be analyzed as equivalent audiences.
- **H2:** Action vs. Sports user ratings — H₀ rejected (p ≈ 0). 
Genres should not be grouped in user preference analysis.

---

## Key Findings

- Most promising platforms for 2017: PS4 and Xbox One
- Japan requires a distinct strategy: portable platforms, RPG focus, 
no Microsoft presence in top 5
- Critic reviews have limited but non-negligible impact on sales
- User scores show almost no correlation with commercial performance

---

## Resources

- 📓 [View Notebook on GitHub](https://github.com/Esparza-Data-An/Market-User-Behavior-Analysis-Global-E-commerce-Gaming-)

---

[← Back to Projects](/projects/)