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

## Data Dictionary

### Patient Demographics (`patient_demographics.csv`)

| Column Name | Description | Data Type |
|-------------|-------------|-----------|
| patient_id | Unique identifier for each patient | Integer |
| age | Age of the patient | Integer |
| gender | Gender of the patient | String |
| location | Geographic location type (Urban/Suburban/Rural) | String |
| insurance_type | Type of insurance coverage | String |
| join_date | Date when patient joined the platform | Date |
| membership_type | Level of membership (Basic/Standard/Premium) | String |
| referral_source | How the patient was referred to the platform | String |
| education_level | Highest level of education completed | String |
| income_bracket | Income level category (Low/Medium/High) | String |
| household_size | Number of people in household | Integer |

### Health Conditions (`health_conditions.csv`)

| Column Name | Description | Data Type |
|-------------|-------------|-----------|
| patient_id | Unique identifier for each patient | Integer |
| health_condition_primary | Main health condition being managed | String |
| condition_severity | Severity of the condition (Mild/Moderate/Severe) | String |
| condition_duration_years | Years since diagnosis | Integer |
| medication_count | Number of medications prescribed | Integer |
| comorbidities_count | Number of additional health conditions | Integer |
| chronic_condition | Whether condition is chronic (Yes/No) | String |
| preventative_care | Whether patient receives preventative care (Yes/No) | String |
| risk_score | Overall health risk assessment (Low/Medium/High) | String |
| care_plan_adherence | Level of adherence to care plan | String |
| last_checkup_date | Date of most recent checkup | Date |

### Engagement Metrics (`engagement_metrics.csv`)

| Column Name | Description | Data Type |
|-------------|-------------|-----------|
| patient_id | Unique identifier for each patient | Integer |
| month | Month of activity data | Integer |
| year | Year of activity data | Integer |
| logins_count | Number of times patient logged in | Integer |
| days_active | Number of days with platform activity | Integer |
| telehealth_appointments | Number of telehealth visits completed | Integer |
| articles_read | Number of educational articles viewed | Integer |
| messages_sent | Number of messages sent to providers | Integer |
| medication_tracking_days | Days medication tracking was used | Integer |
| health_metrics_logged | Number of health metrics recorded | Integer |
| satisfaction_score | User satisfaction rating (0-5) | Float |
| session_duration_avg | Average session length in minutes | Float |
| support_requests | Number of support requests made | Integer |
| feature_usage_count | Number of unique features used | Integer |
| content_shared | Number of items shared from platform | Integer |
| medication_reminders_enabled | Whether medication reminders are active (0/1) | Binary |
| push_notifications_enabled | Whether push notifications are active (0/1) | Binary |
| email_opens | Number of platform emails opened | Integer |
| app_version | Version of app being used | Float |
| device_type | Type of device used (Mobile/Tablet/Desktop) | String |
| survey_responses | Number of surveys completed | Integer |

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


