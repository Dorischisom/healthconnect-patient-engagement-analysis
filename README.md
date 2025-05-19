# HealthConnect+ Patient Engagement & Retention Analysis

![Project_Banner](project_banner/Project_Banner.png)

## Project Overview

HealthConnect+ is a digital health platform that offers telemedicine services, medication management,
health tracking, and educational resources. After 3 years of operation, the company is concerned about
patient engagement and retention rates. This project aims to analyze patient data to understand
engagement patterns, identify churn risk factors, and recommend intervention strategies.

## Business Objectives

1. Identify key factors influencing patient engagement with the platform
2. Analyze patterns of user behavior that predict churn
3. Segment users based on engagement patterns
4. Recommend data-driven intervention strategies for improving retention

## Key Findings

### 1. High-Risk Patient Groups
- **Condition C patients** show the highest churn rate at **82.9%**
- **Rural patients** are **2.4% more likely** to churn than urban patients
- **Word-of-mouth referrals** have **5.5% higher churn** than doctor referrals

![Executive_Summary](Executive_Summary/Executive_Summary.png)

### 2. User Segmentation Results
Machine learning clustering identified **4 distinct user segments** with varying retention patterns:

![User_Segment](User_Segment/Segment_visuals.png)

### 3. Critical Retention Drivers
Feature importance analysis revealed the top factors influencing retention:

![Feature_Importance](Feature_Importance/Feature_importance2.png)

## Business Impact

**Projected Outcomes** from implementing recommended interventions:
- **24% reduction** in overall churn rate (from 74.2% to 56.4%)
- **$2.1M annual revenue** retention
- **15% increase** in patient lifetime value
- **Enhanced patient outcomes** through improved engagement

## 🛠Methodology

This analysis employed a multi-faceted approach:

1. **Data Preprocessing** - Cleaned and merged patient demographics, health conditions, and engagement metrics
2. **Exploratory Analysis** - Identified patterns and correlations in patient behavior
3. **User Segmentation** - K-means clustering and RFM analysis to create actionable segments
4. **Predictive Modeling** - Random Forest classifier for churn prediction (ROC AUC: 0.78)
5. **Feature Engineering** - Created composite engagement scores and behavioral indicators
6. **Intervention Design** - Developed targeted strategies for each user segment

## Technologies Used

- **Python** - pandas, numpy, scikit-learn
- **Machine Learning** - Random Forest, K-means clustering
- **Visualization** - matplotlib, seaborn, plotly
- **Statistical Analysis** - Correlation analysis, RFM modeling
- **Tools** - Jupyter Notebook, Git


