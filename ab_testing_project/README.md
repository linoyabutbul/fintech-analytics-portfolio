
FinTech A/B Testing – Signup & Activation Funnel
This project analyzes an A/B test for a FinTech onboarding funnel, from signup to first transaction.
Objective
Evaluate whether version B of the signup flow improves user activation compared to version A, using:
•	Signup completion
•	Deposit rate
•	First transaction rate
Dataset
•	50K users
•	Columns:
o	user_id
o	version (A/B)
o	viewed_signup
o	clicked_cta
o	completed_signup
o	made_deposit
o	first_transaction
Methods
•	Python (Pandas, NumPy)
•	A/B Testing
•	Statistical significance (Z-test)
•	Funnel and conversion analysis
Key Results
•	Signup Conversion: A → 9.96%, B → 14.37% (+44.1% lift)
•	Deposit Rate: A → 3.91%, B → 5.99% (+53.2% lift)
•	First Transaction Rate: A → 2.13%, B → 3.44% (+62.3% lift)
•	All p-values << 0.05 → results are statistically significant.
Business Conclusion
Version B significantly improves user activation and financial behavior (deposits and transactions).
Recommended to roll out version B to all new users and monitor long-term LTV and monetization.
