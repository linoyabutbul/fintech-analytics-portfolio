# Weekly Cohort Retention Analysis – FinTech User Behavior

This project analyzes user retention behavior over time using **weekly cohorts** based on activity logs of 50,000 FinTech users.

The goal is to understand:
- How users behave after signup  
- When most users churn  
- Which weeks have the strongest retention  
- What insights can be derived to improve activation and long-term engagement  

##  Dataset Overview

The dataset represents **event-level logs**, where each row is a user event:

| Column | Description |
|--------|-------------|
| `user_id` | Unique user identifier |
| `signup_date` | When the user registered |
| `event_date` | Date of the event activity |
| `event_type` | Type of event (signup, login, deposit, transaction, session, failed_payment, card_usage) |

Total users: **50,000**  
Time span: **18 months of user behavior**


##  Analysis Steps

### 1. **Cohort Assignment**
Users were grouped by the week they signed up (`cohort_week`).

### 2. **Event Week Calculation**
For each user event, we calculated the number of weeks since signup (`event_week`).

### 3. **Cohort Pivot Table**
A table was generated showing how many unique users were active each week per cohort.

### 4. **Retention Table**
Retention rates were calculated as:

\[
Retention = \frac{\text{Active Users in Week X}}{\text{Users in Week 0}}
\]

### 5. **Heatmap Visualization**
A full **Weekly Retention Heatmap** was created to observe retention decay patterns across cohorts.

---

## Key Insights

- **Massive drop-off occurs between Week0 → Week1**, reflecting the critical importance of onboarding.  
- Users who remain active up to **Week3 show more stable, long-term retention**.  
- Retention patterns are consistent across cohorts, suggesting stable user behavior over time.  
- Early-life interventions (first 24–72 hours) may significantly improve Week1 retention.  
- Later weeks show gradual and predictable decay — typical of FinTech engagement curves.


##  Summary

This project showcases practical skills in:
- Cohort analysis  
- Retention modeling  
- Behavioral analytics  
- Data visualization (Heatmaps)  
- FinTech product insights  

It is part of the broader **FinTech Analytics Portfolio**, which includes:
- A/B Testing  
- Cohort Retention  
- Additional product & user behavior analyses coming soon.

