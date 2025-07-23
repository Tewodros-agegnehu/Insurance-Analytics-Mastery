#  Insurance Analytics Project – Car Insurance Risk & Premium Modeling

> Predictive Modeling • Risk Segmentation • A/B Testing • Machine Learning  
> **Project Duration:** Dec 25 – Dec 31, 2024

---

##  Overview

This project analyzes historical car insurance policy and claims data to support strategic decision-making in risk segmentation, premium pricing, and product optimization. Through exploratory data analysis, hypothesis testing, and statistical/machine learning modeling, the goal is to provide actionable insights for business impact.

---

## 🎯 Objectives

- Understand and segment **risk profiles** across different customer and location groups.
- Identify **low-risk customer segments** to drive targeted discounts or marketing.
- Conduct **hypothesis testing** on assumptions related to gender, zip codes, and province-level risk.
- Build **predictive models** for estimating total claims and profitability.
- Ensure **reproducibility** and automation using DVC and GitHub Actions.

---

## 📊 Dataset Summary

The dataset spans from **Feb 2014 to Aug 2015**, containing:

- **Client Info:** Gender, Citizenship, Language, Marital Status, VAT status, etc.
- **Vehicle Info:** Make, Model, Year, Cylinders, Capacity, Fleet Size
- **Location:** Province, Postal Code, Cresta Zones (main and sub)
- **Policy Features:** Cover Type, Sum Insured, Term Frequency, Product, Section
- **Claims:** Total Premiums, Total Claims, Capital Outstanding

> Data is versioned and tracked using **DVC** for transparency and reproducibility.

---

## 📁 Project Structure

insurance-analytics/
├── data/ # DVC-tracked raw and processed data
├── notebooks/ # EDA, A/B testing, modeling experiments
├── models/ # Trained model artifacts
├── src/ # Core Python modules and reusable scripts
├── .dvc/ # DVC configuration
├── .github/workflows/ # CI/CD workflows (GitHub Actions)
├── dvc.yaml # DVC pipeline definition
├── requirements.txt # Python dependencies
└── README.md # Project documentation
