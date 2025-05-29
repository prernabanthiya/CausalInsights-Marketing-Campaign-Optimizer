# CausalInsights-Marketing-Campaign-Optimizer
CausalInsights is a data science project designed to uncover the true causal impact of marketing campaigns using modern causal inference techniques. Rather than just predicting behavior, we answer the deeper question: "Did the campaign actually cause this customer to purchase?"

⚠️ Work in Progress: This repo currently focuses on the data science and causal inference module. Frontend and backend components will be added soon.

# **📌 Project Objective**
Traditional machine learning captures correlation, not causation.
This project leverages uplift modeling and treatment effect estimation to:

- Estimate how much a campaign influenced each customer

- Measure the average and individual-level causal impact of marketing efforts

- Identify which customer segments are most responsive to campaigns

# **📊 Dataset**
We use the [Hillstrom Email Marketing Dataset](https://www.kaggle.com/datasets/bofulee/kevin-hillstrom-minethatdata-e-mailanalytics), which simulates a realistic e-commerce campaign scenario with:

- Random assignment to treatment (email) or control group

- Demographic features (age, income, etc.)

- Past purchase history

- Target outcomes: conversion and spending

# **🧠 Core Techniques Used**

✅ Uplift Modeling
Focused on incremental impact estimation, classifying customers into:

- Persuadables – Positively influenced by the campaign

- Sure Things – Would purchase anyway

- Lost Causes – Unaffected by the campaign

- Do Not Disturbs – Negatively influenced by the campaign

✅ Treatment Effect Estimation
- Average Treatment Effect (ATE) – Overall campaign impact

- Conditional Average Treatment Effect (CATE) – Impact across subgroups

✅ A/B Testing Simulation
Uses the dataset’s random assignment structure to simulate a clean A/B test for causal comparisons.

✅ Causal Inference Frameworks
- DoWhy – For encoding causal assumptions, generating causal graphs, identifying estimands, and running refutation tests

- EconML – For advanced estimation of heterogeneous treatment effects using:

- Meta-learners (T-learner, S-learner, X-learner)

- Causal Forests

- Doubly Robust (DR) Learners

# **🚀 Results (Preliminary)**
- Uplift scores successfully separate high-impact customers

- CATE estimation reveals certain age/income groups are more responsive

- Refutation tests support the robustness of causal conclusions

- See notebooks/ and reports/ for detailed plots and metrics.

# **🛠️ Future Work**

- Frontend dashboard (Next.js) for exploring insights interactively

- Flask backend API to serve uplift predictions

- PostgreSQL database to store customer profiles and predictions

- Campaign Optimizer UI to simulate different targeting strategies




