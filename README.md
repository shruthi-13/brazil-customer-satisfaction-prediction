# Customer Satisfaction Prediction — Brazil E-Commerce

**Tools:** KNIME Analytics · Decision Tree · Random Forest · Gradient Boosting  
**Domain:** E-Commerce Analytics · Customer Experience  
**Date:** August – October 2024

---

## Business Problem

A Brazilian e-commerce platform was experiencing customer dissatisfaction but had no systematic way to identify which operational factors were driving negative reviews. The goal: build a predictive model to flag orders likely to receive poor ratings — and surface the root causes driving dissatisfaction.

---

## Dataset

- Customer order data including delivery timing, shipping costs, product categories, and seller location
- Review scores (1–5 stars) as the target variable
- Binary classification: negative review (1–3 stars) vs positive (4–5 stars)

---

## What I Built

### Machine Learning Pipeline in KNIME
- Built and evaluated multiple classification models:
  - Decision Tree
  - Random Forest
  - Gradient Boosting
- Selected best model based on **F1-score** (optimizing for recall of negative reviews)
- Achieved **F1-score of 0.85** on the test set

### Root Cause Analysis
- Analyzed feature importance across models
- Identified the strongest drivers of customer dissatisfaction
- Translated findings into operational recommendations for the business

---

## Results

| Metric | Value |
|---|---|
| Best F1-Score | **0.85** |
| Models Evaluated | Decision Tree, Random Forest, Gradient Boosting |
| Platform | KNIME Analytics |
| Target | Negative review prediction (binary) |

---

## Key Findings

| Driver | Impact |
|---|---|
| **Delivery Delays** | #1 driver of poor ratings — late deliveries strongly predict 1–2 star reviews |
| **Shipping Costs** | #2 driver — high shipping cost relative to product price triggers dissatisfaction |
| **Product Category** | Certain categories (electronics, furniture) show disproportionately high complaint rates |
| **Seller Location** | Orders from distant sellers correlate with longer delivery times and lower scores |

---

## Business Recommendations

1. **Prioritize on-time delivery SLAs** — even 1-day delays significantly increase negative review probability
2. **Offer free or capped shipping** on high-risk categories to reduce cost-driven dissatisfaction
3. **Flag high-risk orders proactively** using the model — trigger customer support outreach before reviews are submitted
4. **Review seller performance by region** — distant sellers with poor delivery records should face stricter onboarding criteria

---

## Skills Demonstrated

- End-to-end ML pipeline in KNIME (data prep → modeling → evaluation)
- Multi-model comparison and F1-score optimization
- Business root cause analysis from feature importance
- Translating model outputs into operational e-commerce strategy
