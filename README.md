# Credit Risk Intelligence & Fairness System

<img width="1344" height="768" alt="image" src="https://github.com/user-attachments/assets/f0149399-e08f-49cb-99e6-dfbc19638889" />


## Introduction
In the banking sector, identifying **High Risk** loan applicants is crucial for financial stability. This project analyzes historical credit data to predict the likelihood of borrower default. By leveraging **Machine Learning**, we developed a system that provides **probability-based risk assessments** while ensuring **transparency** and **ethical fairness**.

---

## Objectives
- **Minimize Financial Loss:** Develop a classification algorithm that prioritizes **Recall**, catching as many potential defaults as possible.  
- **Ensure Transparency:** Implement **Explainable AI (XAI)** to justify why an applicant is labeled high risk.  
- **Audit for Fairness:** Perform bias checks to ensure the model does not discriminate based on protected attributes like **Gender** or **Age**.

---

## The Data
We used the **Statlog (German Credit Data)**, a standard dataset for credit risk research. It contains **1,000 entries** with features such as credit history, loan purpose, employment status, and personal demographics.  

Key points:  
- Engineered a realistic **Risk** target to simulate high-stakes lending.  
- Introduced stochastic noise to reflect real-world unpredictability.

---

## Features
- **Dual-Model Comparison:** Logistic Regression (interpretable) vs. Support Vector Machines (SVM) to balance transparency and complex decision boundaries.  
- **Class Imbalance Correction:** Applied **balanced class weighting** to ensure the minority **Bad Risk** cases are adequately captured.  
- **Ethical AI Audit:** Custom fairness checks visualize prediction rates across demographics.  
- **Feature Importance Visualization:** Clear breakdown of top drivers of credit risk (e.g., **Loan Duration**, **Credit Amount**).

---

## How It Works
1. **Data Ingestion:** Cleans raw application data; missing values are categorized as "unknown."  
2. **Preprocessing:** Encodes categorical data and standardizes numerical features (Age, Amount, Duration) using **StandardScaler**.  
3. **Risk Analysis:** Algorithm generates a **Risk Probability Score** for each application.  
4. **Decision & Insight:** Outputs a final status (**LOW RISK ✅** or **HIGH RISK 🚩**) and provides **Feature Importance** to explain the key drivers of the decision.

---

## Project Performance
- **F1-Score:** 0.90+ (high balance between Precision and Recall)  
- **Recall:** ~0.91 (successfully identifies 9 out of 10 potential defaults)  
- **Transparency:** 100% explainable coefficients via Logistic Regression
