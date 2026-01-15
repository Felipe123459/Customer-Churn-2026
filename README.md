# Customer-Churn-2026
## Overview
Customer churn is a major challenge for financial institutions, as retaining existing customers is significantly more cost-effective than acquiring new ones.  
This project analyzes customer churn using a banking dataset to identify key behavioral and financial drivers of churn and to build predictive models that estimate churn risk.

The project combines exploratory data analysis, customer segmentation, and machine learning to provide both **descriptive insights** and **predictive capability**.

---

## Objectives
- Identify the primary factors influencing customer churn
- Segment customers using unsupervised learning (K-Means clustering)
- Build and compare churn prediction models
- Translate findings into actionable business insights

---

## Dataset
- **Source:** Kaggle – Customer Churn Dataset  
- **Key Features:**
  - Age
  - Balance
  - Estimated Salary
  - Credit Score
  - Number of Products
  - Geography
  - Tenure
  - Activity Status
  - Churn Indicator (Exited)

---

## Methodology

### Exploratory Data Analysis (EDA)
- Analyzed churn distribution across demographics and financial features
- Visualized churn by geography, activity status, and product ownership
- Identified correlations and non-linear relationships between features

### Customer Segmentation
- Preprocessed numerical features and applied **K-Means clustering**
- Analyzed cluster-level behavior to identify high-risk customer segments

### Predictive Modeling
- Implemented two classification models:
  - Logistic Regression
  - Random Forest
- Evaluated models using:
  - Confusion matrices
  - False negative rates
- Selected the optimal model based on business impact

---

## Key Findings
- **Age** is the strongest predictor (0.23 feature importance), with customers 60+ showing 40% higher churn rates
- **Inactive members** churn nearly **2× more** than active members
- **Germany** exhibits the highest churn rate (~34%) despite a smaller customer base
- Customers with **more products** are significantly less likely to churn
- Customers near the **median salary range** show lower churn probability
- Cluster 1 (younger, multi-product customers) shows **14.6%** churn vs 23-24% in other segments
---

## Model Performance
- The **Random Forest model** outperformed Logistic Regression
- Random Forest Accuracy: 72.1% (optimized for recall)
- Catches 64.6% of actual churners vs 46.2% with the baseline model
- Random Forest produced a **lower false negative rate**, which is critical in churn prediction because failing to identify a customer who will leave results in lost revenue
- Feature importance analysis aligned with EDA findings, reinforcing model reliability

---

## Tools & Technologies
- Python (Pandas, NumPy, Scikit-learn)
- Tableau (interactive dashboard and visualization)
- Jupyter Notebook
- GitHub for version control

---

## Deliverables
- Interactive Tableau dashboard summarizing churn drivers and customer segments
- Machine learning models for churn prediction
- Feature importance analysis for interpretability
<img width="1708" height="1014" alt="image" src="https://github.com/user-attachments/assets/cc421664-b9ee-4486-984a-244dc766758b" />

---


## Business Value
This analysis helps financial institutions:
- Identify high-risk customers early
- Target retention strategies more effectively
- Allocate marketing and customer service resources based on churn risk

## Future Improvements
- Incorporate time-based features if available
- Tune model hyperparameters using cross-validation
- Explore survival analysis for churn timing
