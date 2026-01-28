# 📘 Credit Card Churn Classification  
Predict customer churn for a credit-card issuer using machine learning classification models.

---

## 🔍 Overview  
- **Goal:** Build a predictive model to classify whether a customer will churn (attrite) based on demographic, account, and transaction behavior.  
- **Problem Type:** Binary Classification  
- **Dataset:** Public credit-card churn dataset (~10k+ customers) combining demographic info, account tenure, and transaction activity.

---

## 🧭 Context  
Customer churn significantly impacts profitability for credit-card companies.  
Identifying high-risk customers enables proactive retention strategies, such as targeted offers, improved onboarding, or engagement campaigns, thus reducing revenue loss and improving customer lifetime value.  

This project demonstrates an end-to-end machine learning workflow to predict churn and extract meaningful behavioral insights.

---

## 📊 Data Summary  
- **Target Variable:** `Attrition_Flag` (Existing Customer vs. Attrited Customer)  
- **Key Features:**  
  - **Demographics:** age, gender, dependents, education level, marital status, income category  
  - **Account Details:** card category, credit limit, months on book, relationship count  
  - **Behavior & Usage:** total transaction count, transaction amount, revolving balance, utilization ratio, change in transaction volume, inactivity periods  
- **Data Issues:**  
  - Noticeable **class imbalance** (approx. 16% churn)  
  - Feature distributions vary widely → scaling needed  
  - Mix of categorical and continuous variables

---

## 🛠 Methods & Concepts Used  
- **Preprocessing:**  
  - Label encoding / one-hot encoding  
  - Standardization of numerical features  
  - Handling outliers and skewness

- **Resampling (Class Balancing):**  
  - Techniques such as **downsampling (RandomUnderSampler)** or **oversampling (SMOTE)** to mitigate imbalance

- **Modeling:**  
  - Gradient Boosting
  - AdaBoost
  - XGBoost
  - Model comparison using classification metrics

- **Techniques:**  
  - Train/test split  
  - Cross-validation  
  - Hyperparameter tuning  
  - Feature importance analysis  

---

## 💡 Actionable Insights  
- Use the model to **identify customers with a high likelihood of attrition** and target them proactively with tailored offers. For example, provide exclusive discounts or partner-retailer promotions only to customers flagged as high-risk, reducing churn while minimizing the cost of broad, untargeted incentives.

- **Enhance credit-card benefits** to encourage increases in transaction amount and transaction count—two of the most influential factors in the model. This may include offering additional cashback, bonus points, or temporary rewards to customers showing low activity.

- Conduct **qualitative research** with recently churned customers to understand the reasons behind reduced transaction activity and account closure. These insights can help identify pain points and inform improvements to customer experience or product design.

- **Collect and incorporate fee-related data** (such as annual fees or service charges) into future iterations of the model. This will allow analysis of the relationship between credit usage and fees and may improve predictive performance.


---

## 👤 Author  
**Henrique Barbosa**  
GitHub: https://github.com/henriqueb-data/
