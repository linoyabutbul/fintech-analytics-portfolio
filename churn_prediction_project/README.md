# Churn Prediction – FinTech User Behavior Modeling

This project builds a **Machine Learning model** to predict user churn in a FinTech product using a realistic dataset of 50,000 users.

The goal is to identify which users are likely to churn and understand **why**, using feature analysis and business insights.

---

## 📊 Dataset Overview

Each row represents a user with behavior-based and demographic features:

| Feature | Description |
|--------|-------------|
| user_id | Unique user identifier |
| age | User age |
| signup_date | Date when the user registered |
| last_active_date | Last date the user opened the app |
| days_since_last_active | Number of inactive days |
| total_transactions | Number of transactions performed |
| total_deposits | Number of deposits |
| avg_transaction_amount | Average transaction amount |
| session_count | Number of app sessions |
| device_type | iOS / Android / Web |
| is_premium | 1 = premium subscriber |
| churn | 1 = churned, 0 = active |

 **Churn definition:**  
A user who has been inactive for **more than 45 days** is labeled as churned.

---

##  Modeling Approach

### Steps Performed:
1. **Data preprocessing**
   - Scaling numeric features  
   - One-Hot Encoding for categorical features  
   - Building a preprocessing pipeline  

2. **Train/Test Split**
   - 75% for training  
   - 25% for evaluation  

3. **Model Training**
   **Logistic Regression** was selected due to interpretability and industry standard in churn prediction.

4. **Model Evaluation**
   - Confusion Matrix  
   - Precision, Recall, F1-score  
   - ROC Curve + AUC  

---

## 📈 Key Evaluation Metrics

### ROC Curve
AUC score: **1.000**  
This indicates that the model separates churners from non-churners *perfectly*, due to highly predictive behavioral features.

---

## 🔥 Feature Importance (Top 8 Predictors)

| Feature | Effect |
|--------|--------|
| **days_since_last_active** | Strongest churn indicator |
| avg_transaction_amount | Low avg → higher churn |
| device_type_web | Web users churn more |
| total_deposits | Fewer deposits → higher churn |
| is_premium | Premium users churn less |
| device_type_ios | iOS churns slightly less than Android |
| age | Older users churn slightly less |
| session_count | More sessions → lower churn |

---

##  Business Insights

1. **Inactivity is the strongest churn driver**  
   Users inactive for long periods have extremely high churn risk.  
   → Implement push reminders & re-engagement flows.

2. **Low financial activity = high churn**  
   Users with few deposits/transactions tend to leave.  
   → Offer first-deposit bonuses or simple starter tasks.

3. **Web users churn significantly more**  
   → UX for web users needs improvement.

4. **Premium users are very loyal**  
   → Excellent segment for upselling.

5. **High engagement reduces churn**  
   Session count is a strong retention factor.  
   → Encourage habit-forming behaviors.


##  Summary

This project demonstrates:
- Predictive modeling (classification)  
- ML pipelines with preprocessing  
- Behavioral feature analysis  
- Understanding of churn drivers  
- Real-world FinTech insights  

