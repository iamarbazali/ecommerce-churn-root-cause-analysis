# Ecommerce Churn Root Cause Analysis

A business analytics project to explain why churn changed and which customer segment is most at risk in a subscription e-commerce business.

# Project Summary

This project studies churn in a Kaggle e-commerce customer dataset with about 5,600 rows and 20 columns. The goal is not to build a dashboard. The goal is to find the main churn drivers, test them with data, and turn them into one clear recommendation for leadership.

# Business Problem

The business saw churn rise in one quarter. The main question was not only what changed, but why it changed and what action the business should take next.

# Core business goal:
Identify the highest risk customer segment and recommend one focused retention action.

# What I found

The data does not support a strong Q3 churn spike in the cleaned dataset. Churn is more strongly linked to customer experience signals.

Strongest churn signals found so far:
- Customers who complained churned more.
- Customers with lower satisfaction churned more.
- Customers in higher city tiers showed higher churn.
- Some missing value patterns also carried churn signal, especially in columns tied to usage and customer behavior.

What this means:
- The main churn driver is not quarter alone.
- The likely root issue is customer experience quality.
- Service friction, complaints, and low satisfaction appear more important than calendar timing.

# Analysis approach

Phase 1. Business thinking
- Defined churn in business terms.
- Estimated churn cost.
- Wrote five hypotheses before looking at the data.

Phase 2. Data cleaning and EDA
- Checked missing values.
- Handled missing numeric values with multiple imputation.
- Added missingness flags.
- Compared churn across imputed versions to test stability.

Phase 3. Segment and driver analysis
- Compared churn by complaint, satisfaction, city tier, and missingness signals.
- Checked churn by quarter.
- Tested whether the quarter spike really existed in the cleaned data.

# Current conclusion

Based on the data explored so far, churn appears to be driven more by customer experience than by quarter timing.

Most important patterns:
- Complaint rate is much higher among churned customers.
- Lower satisfaction aligns with higher churn.
- City tier differences also matter.
- Missing values in selected behavioral columns may signal hidden churn risk.

# Business recommendation

Focus retention on customers showing poor experience signals.

# Recommended action:
Build a targeted retention workflow for customers who complain, show low satisfaction, or have weak engagement signals such as low order activity or long gaps since last order.

# Why this matters:
- These customers are more likely to churn.
- They are easier to intervene on than broad quarter based segments.
- A focused action is more practical than a broad churn campaign.

# Project status

- Phase 1, Business thinking and hypothesis writing, Done
- Phase 2, Data cleaning and EDA, Done
- Phase 3, Statistical testing and logistic regression, Done
- Phase 4, K Means clustering and segment profiling, Done
- Phase 5, Recommendation writing and presentation, In Progress

# Tech stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit learn
- Jupyter Notebook

# Files in this repo

- problem_definition.txt, business context and hypotheses
- root_cause.ipynb, analysis notebook
- E-Commerce-Dataset.xlsx, source data

# Portfolio summary

Identified the main churn drivers in a subscription e-commerce dataset using structured hypothesis testing, missing value analysis, and customer segmentation. The analysis shows that churn is more closely tied to customer experience than to quarter timing, and points to a targeted retention action for at risk customers.
