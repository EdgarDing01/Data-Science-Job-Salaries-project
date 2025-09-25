# Overview

**Background**

This dataset contains **job salary records for Data Science roles worldwide**, covering multiple years and diverse working arrangements.
It provides information on **job titles, experience levels, employment types, company sizes, locations, remote work ratios**, and most importantly, **standardized salaries (in USD)**.

Given the global demand for data professionals, this dataset is valuable for **analyzing salary trends**, **understanding factors that drive compensation**, and **supporting career or HR planning decisions**.

**Goal of the Project**

Build a machine learning model to:

* **Predict salary (USD)** based on job, experience, and company attributes
* Identify **key drivers of compensation** (experience, company size, remote ratio, etc.)
* Provide insights for **job seekers and employers** to make data-driven career and hiring decisions

**Key Features**

| Feature Name         | Description                                                          |
| -------------------- | -------------------------------------------------------------------- |
| `work_year`          | Year of observation                                                  |
| `experience_level`   | Level of experience (Entry, Junior, Senior, Executive)               |
| `employment_type`    | Type of employment (Full-time, Part-time, Contract, Freelance)       |
| `job_title`          | Role of the employee (e.g., Data Scientist, ML Engineer, Analyst)    |
| `salary`             | Salary amount in the original currency                               |
| `salary_currency`    | Currency of the reported salary                                      |
| `salary_in_usd`      | Salary standardized to USD (**target variable**)                     |
| `employee_residence` | Country of residence of the employee                                 |
| `remote_ratio`       | Degree of remote work (0 = on-site, 50 = hybrid, 100 = fully remote) |
| `company_location`   | Country where the company is based                                   |
| `company_size`       | Size of the company (S = small, M = medium, L = large)               |

**Files Provided**

* `ds_salaries.csv`: Main dataset containing job-related attributes and salary information.

**Project Objective**

The goal of this notebook is to **model and predict data science salaries**, helping to:

* Benchmark salaries across roles, levels, and geographies
* Explore the effect of remote work and company size on pay
* Support fair compensation strategies in the job market
* Provide insights for career planning and HR analytics

**Key Steps**

* **Exploratory Data Analysis (EDA):** <br>
  Study salary distribution by job title, location, company size, remote ratio, and experience level.

* **Feature Engineering:**
  Encode categorical variables, normalize salaries, and create derived features (e.g., region grouping).

* **Modeling:**
  Train and compare multiple models:

  * Linear Regression
  * Random Forest Regressor
  * XGBoost / LightGBM
  * Ensemble approaches

* **Evaluation Framework:**
  Use cross-validation and evaluate with:

  * R² (Coefficient of Determination)
