# Predictive Modelling for Pricing and Subscription Targeting

## Overview
This project is a combined predictive analytics portfolio focused on building, comparing, and evaluating models for two business problems:
1) Predicting whether a bank customer will subscribe to a term deposit (classification).
2) Predicting average airfare for a new airline route and estimating the impact of Southwest entering that route (regression + scenario simulation).

## Case 1 — Term Deposit Subscription Prediction (Classification)
### Goal
Improve telemarketing efficiency by predicting which customers are most likely to subscribe to a term deposit, prioritising “yes” detection to maximise ROI.

### Process
- Followed CRISP-DM: business understanding → data understanding → preparation → modelling → evaluation → deployment proposal.
- Addressed class imbalance using oversampling and evaluated multiple models.

### Data Preparation Highlights
- Verified missing values were not present.
- Removed redundant date fields and applied categorical encoding.
- Applied targeted outlier handling with domain reasoning.
- Used scaling (normalization/standardization) where required.
- Split into train/test and oversampled the minority “yes” class.

### Models Compared
Logistic Regression, Classification Tree, Random Tree, Neural Network, Bagging, Boosting.

### Outcome
Boosting (Decision Trees) delivered the strongest overall performance (highest recall and F1 for “yes”), making it the most suitable model for campaign targeting.

## Case 2 — Airfare Prediction for New Routes (Regression)
### Goal
Forecast average fare for a new route using demographic, geographic, and market variables, and quantify expected fare change if Southwest serves the route.

### Process
- Followed a SEMMA-style workflow: explore → preprocess → encode → partition → model → assess.
- Benchmarked multiple models using SSE, RMSE, MAD, and R².

### Models Compared
Linear regression, regression trees (pruned), neural networks, bagging, and boosting regression.

### Outcome
Boosting regression achieved the best predictive accuracy (lowest RMSE, highest R²). Scenario testing showed Southwest service significantly reduces predicted fares. A reduced “pre-launch only” model was also evaluated to reflect which predictors are available before operations begin, and performance trade-offs were documented.

## What this demonstrates
End-to-end predictive modelling with structured methodologies, practical preprocessing (imbalance + outliers + encoding), transparent model comparison using metrics, and business-driven interpretation through scenario analysis.
