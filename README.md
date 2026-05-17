# Ecommerce Churn Root Cause Analysis

A business analytics project investigating why monthly churn jumped from 8% to 14% in one quarter for a subscription e-commerce company.

This is not a dashboard project. The output is a single data-backed recommendation to leadership, built through structured hypothesis testing, statistical validation, and customer segmentation.

---

## Project Structure

| Phase | Task | Status |
|-------|------|--------|
| Phase 1 | Business thinking and hypothesis writing | Done |
| Phase 2 | Data cleaning and EDA | In Progress |
| Phase 3 | Statistical testing and logistic regression | Pending |
| Phase 4 | K-Means clustering and segment profiling | Pending |
| Phase 5 | Recommendation writing and presentation | Pending |

---

## Business Problem

**Churn rate:** 8% to 14% in one quarter  
**Dataset:** E-Commerce Customer Churn (Kaggle, ~5,600 rows, 20 columns)  
**Goal:** Identify the root cause segment and propose one targeted retention action

---

## Phase 1: Business Thinking

Before writing any code, three core questions were answered:

1. **What is churn here?** A customer who stopped ordering or cancelled their subscription, either voluntarily (dissatisfaction, competitor) or involuntarily (payment failure, delivery issue).

2. **What does churn cost?** Three layers: lost recurring revenue, lost upsell probability (existing customers convert at 65% vs 13% for new prospects), and increased CAC since replacing a customer costs 5x more than retaining one.

3. **What does a useful answer look like?** A specific segment + a specific cause + one action.

---

## Hypotheses

Five hypotheses written before any data exploration to avoid fishing for random correlations:

1. Customers with low tenure + low satisfaction have a higher churn rate
2. Customers with low app hours + low satisfaction are more likely to churn
3. Customers with low tenure + low order count are likely to churn
4. Customers with high device count + low satisfaction are more likely to churn
5. Customers with high days since last order + low order count are likely to churn

Each hypothesis includes a primary metric, secondary metrics, and support metrics defined upfront.

---

## Tools

- Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)
- Jupyter Notebook

---

## Files

- `problem_definition.txt` — Business context, cost of churn, and 5 hypotheses with metrics
- `root_cause.ipynb` — Analysis notebook (updated progressively)
- `E-Commerce-Dataset.xlsx` — Source dataset

---

## Portfolio Note

Project description: *Identified the highest-risk churn segment in a subscription e-commerce dataset using statistical testing, logistic regression, and K-Means clustering. Proposed a targeted retention intervention based on root cause analysis, not descriptive stats.*
