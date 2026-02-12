# Customer_Churn_Project

## SyriaTel Customer Churn Prediction

Python | Scikit-Learn | Machine Learning | Classification

A complete machine learning project for predicting customer churn at SyriaTel using classification models and actionable business insights.

---

## Project Overview

This project implements a classification model to predict whether a customer is likely to churn (leave SyriaTel’s services). The project includes data cleaning, feature engineering, handling class imbalance, model training, evaluation, feature importance, and business recommendations. The goal is to help SyriaTel identify high-risk customers and improve retention strategies through data-driven decisions.

---

## Key Features

* EThe project's flow: Data preprocessing → Modeling → Evaluation → Insights
* Multiple algorithms: Logistic Regression, Random Forest, Decision Tree
* Handling class imbalance with SMOTE
* Model comparison using Recall, Precision, and F1-score
* Feature importance analysis for business interpretation
* Actionable recommendations to reduce churn

---

## Project Structure

```
SyriaTel_Customer_Churn/
│
├── Data/
│   └── Customer_Churn.csv          
├── SyriaTel_Churn_Analysis.ipynb   
├── README.md                 
                
```

---

## Dataset Information

* **Source:** [SyriaTel Churn Dataset on Kaggle](https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset)
* **Records:** ~3,300 customers
* **Features:** Call usage, subscription plans, charges, service interactions
* **Target:** Churn (1 = Yes, 0 = No)

**Key Feature Categories:**

* Call Usage: Day, Evening, Night, and International minutes & charges
* Account Info: Area code
* Customer Support: Number of service calls
* Subscription Plans: International plan, Voice mail plan

---

## Modeling Overview

**Models Trained:**

* Logistic Regression (Baseline)
* Logistic Regression (Tuned)
* Random Forest
* Decision Tree

**Model Performance Summary:**

| Model                     | Recall | Precision | F1 Score       |
| ------------------------- | ------ | --------- | -------------- |
| Logistic Regression       | 0.77   | 0.32      | 0.44           |
| Tuned Logistic Regression | 0.77   | 0.32      | 0.44           |
| Random Forest             | 0.69   | 0.76      | 0.73           |
| Decision Tree             | 0.72   | 0.45      | 0.55           |

**Best Model:** Random Forest (achieves the best balance of recall and precision based on F1-score)

---

## Key Insights

* Top predictors of churn: **Total Day Charge, Total Day Minutes, Total Evening Charge, Customer Service Calls**
* High call charges and frequent customer service interactions increase the likelihood of churn
* Billing patterns and service experiences are stronger drivers of churn than plan subscription features

---

## Recommendations

1. **Improve Customer Support:** Resolve issues faster, reduce repeated calls, and provide proactive follow-ups.
2. **Monitor High-Spending Customers:** Offer loyalty discounts, personalized plans, or bundled packages to retain high-billing customers.
3. **Reassess Pricing Strategies:** Especially international and day call charges to reduce dissatisfaction.
4. **Implement Early Churn Detection:** Deploy the Random Forest model to identify at-risk customers early.
5. **Continuous Monitoring:** Regularly retrain models and track customer behavior to maintain predictive key metrics.

---

## Conclusion

The **Random Forest model** performed best for predicting customer churn based on F1-score, balancing recall and precision effectively. Feature importance analysis shows that **billing-related factors and customer support interactions** are the strongest drivers of churn. This analysis enables SyriaTel to intervene proactively and reduce revenue loss while improving customer retention.

---



