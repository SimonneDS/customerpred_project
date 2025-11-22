# Telecom Customer Churn Prediction — Machine Learning Project

## Project Overview

This project aims to develop a **predictive model for customer churn** using real-world telecom data.  
The primary goal was to identify key factors contributing to customer attrition and design a data-driven strategy to **reduce churn rates** and improve customer retention.

---

## Objectives

- Build a robust classification model capable of predicting customer churn.  
- Achieve a minimum **AUC-ROC of 0.75** and a stretch goal of **≥ 0.85**.  
- Provide actionable business insights through **feature importance analysis**.  
- Support proactive decision-making for customer retention strategies.

---

## Dataset

The dataset contains customer information, service usage patterns, and contract details from a telecom company.

**Main features:**
- `customerID`: Unique customer identifier  
- `gender`, `SeniorCitizen`, `Partner`, `Dependents`  
- `tenure`: Number of months the customer has stayed  
- `PhoneService`, `InternetService`, `StreamingTV`, `StreamingMovies`  
- `Contract`, `PaperlessBilling`, `PaymentMethod`  
- `MonthlyCharges`, `TotalCharges`  
- `Churn`: Target variable (Yes/No)

**Data preprocessing included:**
- Handling missing values and outliers  
- Encoding categorical features  
- Engineering new features (e.g., tenure grouping, service bundles)  
- Standardizing numerical variables  

---

## Methodology

1. **Exploratory Data Analysis (EDA)**  
   - Explored customer demographics, service types, and churn distribution.  
   - Visualized correlations and service combinations impacting churn.

2. **Feature Engineering**  
   - Created tenure categories and binary service flags.  
   - Encoded categorical variables using one-hot encoding.  
   - Addressed class imbalance where necessary.

3. **Model Training and Evaluation**  
   - Tested multiple models: Logistic Regression, Random Forest, and LightGBM.  
   - Tuned hyperparameters using cross-validation and grid/random search.  
   - Evaluated with metrics: **AUC-ROC, Accuracy, Precision, Recall, F1-score**.

4. **Model Selection**  
   - The final model chosen was **LightGBM**, offering the best performance and interpretability.

---

## Model Performance

| Metric | Result |
|:--|:--:|
| **AUC-ROC** | 0.8451 |
| **Accuracy** | 0.8034 |
| **Precision** | 0.79 |
| **Recall** | 0.81 |

**Goal achieved:** The model exceeded the target AUC-ROC of 0.75, reaching **0.8451**.  
This confirms strong predictive performance and reliable identification of at-risk customers.

---

## Key Insights

- **Contract Type (Month-to-Month)**: Strongest churn predictor — flexible customers are more likely to leave.  
- **Tenure**: Customers with shorter tenure show significantly higher churn risk.  
- **InternetService (Fiber Optic)**: Higher churn rates suggest dissatisfaction with value or service stability.  

These findings align with industry trends, confirming that **customer engagement and pricing strategy** are critical drivers of retention.

---

## Strategic Recommendations

1. **Targeted Incentives**  
   Offer tailored discounts or upgrades for month-to-month customers, especially those using Fiber Optic plans.

2. **Proactive Retention System**  
   Develop automated churn alerts to flag high-risk customers early.

3. **Service Quality Audits**  
   Investigate technical or satisfaction issues related to Fiber Optic plans.

4. **Customer Lifecycle Management**  
   Implement engagement programs for new customers within their first 6 months.

---

## Future Improvements

- Integrate **customer feedback and sentiment analysis** for deeper insights.  
- Deploy the model into a **real-time dashboard** for monitoring churn probability.  
- Conduct **A/B testing** to measure the impact of retention campaigns.

---

## Tools and Libraries

- **Python** (Pandas, NumPy, Matplotlib, Seaborn)  
- **Scikit-learn** (Metrics, Model Selection)  
- **LightGBM** (Final model)  
- **Jupyter Notebook** (Development environment)

---

## Author

**Simonne Andrea Arancibia Cárdenas**  
Data Scientist | Data Analyst | Problem Solver  

📍 Based in Australia | 🌐 [LinkedIn](https://www.linkedin.com/in/simonne-andrea-arancibia-c%C3%A1rdenas-72943b163) | 💻 [GitHub](https://github.com/SimonneDS)

---

## Summary

This project successfully demonstrates how **machine learning can drive customer retention strategies** by identifying at-risk clients before they churn.  
The LightGBM model empowers the telecom company to move from reactive responses to **data-driven proactive engagement**, ultimately improving customer loyalty and business profitability.
