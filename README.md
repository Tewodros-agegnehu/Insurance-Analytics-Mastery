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


---

##  Key Tasks

### Task 1 – Git & Exploratory Data Analysis (EDA)

- Set up Git version control and GitHub repository
- Create development branches per task
- Perform descriptive statistical analysis
- Create insightful visualizations (univariate, bivariate, multivariate)
- Assess missing values and data quality

>  Branch: `task-1`

---

### Task 2 – Data Version Control (DVC)

- Initialize DVC in the repo
- Track raw data files using `dvc add`
- Configure and push to a local DVC remote
- Ensure reproducibility across environments

>  Branch: `task-2`

---

### Task 3 – A/B Hypothesis Testing

Test the following hypotheses:

- Risk does not differ across provinces
- Risk does not differ across zip codes
- No significant profit margin differences by zip code
- No risk difference between men and women

> Methods: T-test, Z-test, Chi-squared test  
> Result interpretation based on p-values and effect sizes

>  Branch: `task-3`

---

### Task 4 – Statistical Modeling

- **Preprocessing:** Encoding, missing value treatment, feature creation
- **Modeling Techniques:**
  - Linear Regression
  - Random Forest
  - XGBoost
- **Evaluation Metrics:** RMSE, MAE, Precision, Recall, F1-score
- **Model Interpretation:** SHAP / LIME for explaining key feature effects

>  Branch: `task-4`

---

##  CI/CD Pipeline

CI/CD is implemented with **GitHub Actions** to automate:

- Code quality checks (linting)
- Data pipeline testing
- Notebook execution validation
- Trigger on push and PR to main

> YAML workflow file available in `.github/workflows/ci.yml`

---

##  Learning Outcomes

- Hands-on practice with data cleaning, EDA, and statistical testing
- Practical A/B test design and analysis for business decisions
- Application of regression and ensemble modeling for claim prediction
- Use of DVC for reproducible machine learning pipelines
- CI/CD pipeline setup for ML workflows

---


##  References

- [DVC Documentation](https://dvc.org/doc)
- [Understanding A/B Testing](https://www.optimizely.com/optimization-glossary/ab-testing/)
- [Random Forest Algorithm – Analytics Vidhya](https://www.analyticsvidhya.com/blog/2021/06/random-forest-algorithm/)
- [XGBoost Explained](https://www.analyticsvidhya.com/blog/2018/09/an-end-to-end-guide-to-understand-the-math-behind-xgboost/)
- [SHAP: Explain Model Predictions](https://shap.readthedocs.io/en/latest/)

---

##  Get Involved

-  [Raise an Issue](https://github.com/your-org/Insurance-Analytics-Mastery/issues)
-  Submit a [Pull Request](https://github.com/your-org/Insurance-Analytics-Mastery/pulls)
-  Clone and explore locally

```bash
git clone https://github.com/your-org/Insurance-Analytics-Mastery.git
cd Insurance-Analytics-Mastery
pip install -r requirements.txt
