Internship Compensation Intelligence Analysis

📌 Overview

This project analyzes 649 U.S. data-related internship listings to benchmark compensation trends and evaluate the impact of geography, role type, company rating, and remote status on salary variation.

Salaries were standardized from mixed hourly and annual formats into comparable monthly compensation estimates, followed by feature engineering, correlation analysis, and multivariate regression modeling.

The objective was to understand which factors meaningfully influence internship pay and to demonstrate structured analytics workflow using real-world job market data.

Dataset

Source: Kaggle – Data Science & Analytics Internship Listings (2024–2025)

Total Listings: 649

Valid Salary Observations: 503

Fields Used:

Company

Company Score

Job Title

Location

Salary

🛠 Technical Approach
1️⃣ Data Cleaning & Normalization

Converted hourly wages to monthly equivalents (40 hrs/week assumption)

Converted annual salaries to monthly values

Standardized mixed formats for comparability

2️⃣ Feature Engineering

Categorized roles (Data Scientist, Data Engineer, Analyst, ML Engineer)

Extracted state from location

Created binary remote indicator

Applied one-hot encoding for categorical modeling

3️⃣ Exploratory Analysis

Median salary by state

Salary by role category

Remote vs on-site comparison

Company rating segmentation

4️⃣ Statistical Analysis

Correlation heatmaps

Multivariate linear regression (train-test split)

📊 Key Findings

Median monthly salaries ranged from approximately $5,100 to $8,400 across top states.

Role type showed stronger salary association than company rating.

Pairwise correlations between individual features and salary were modest (< 0.10), indicating compensation is influenced by multiple interacting factors.

Initial regression using only rating and remote status showed negligible explanatory power (R² ≈ 0.002).

After incorporating role and state via one-hot encoding, model performance improved, demonstrating the importance of proper feature engineering.

📈 Visualizations
Salary by State

<img width="630" height="470" alt="image" src="https://github.com/user-attachments/assets/92d4c207-2c6a-4a53-97d8-4cc9112ce169" />


Salary by Role Category

<img width="630" height="469" alt="image" src="https://github.com/user-attachments/assets/02b78958-3990-49f0-a5bb-b8e1d1103947" />


Top Correlated Features with Salary

<img width="609" height="790" alt="image" src="https://github.com/user-attachments/assets/7b010fdd-825f-4a1c-bdfb-21503544f7e5" />


📚 Tools & Libraries

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

🎯 Why This Project Matters

This analysis demonstrates the ability to:

Clean and standardize messy real-world data

Engineer meaningful categorical features

Apply statistical reasoning responsibly

Interpret weak vs strong model signals correctly

Build a structured end-to-end analytics workflow

The project reflects practical business analytics application to labor market compensation benchmarking.
