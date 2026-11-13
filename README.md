# Telco Customer Churn Analysis

### Customer Retention Analysis Using Excel, Power Query and Power BI

## 1. Project Overview

This project focuses on analysing customer churn in a telecommunications company to understand customer attrition patterns and identify customer segments with higher churn rates.

The analysis uses customer demographics, service subscriptions, contract types, payment methods, customer tenure and billing information to explore factors associated with customer churn.

Excel Power Query was used for data cleaning and preparation, while Power BI was used to create KPI measures, interactive visualisations and a customer churn dashboard.

The primary objective is to generate meaningful business insights that can help the company understand customer behaviour and develop effective customer retention strategies.

## 2. Business Problem

Customer churn is a major challenge for telecommunications companies because losing customers can affect recurring revenue and long-term business growth.

The company needs to understand:

- What percentage of customers are leaving?
- Which contract types have the highest churn?
- How does customer tenure relate to churn?
- Which internet service categories experience higher churn?
- Does technical support subscription relate to customer retention?
- Which payment methods are associated with higher churn?

This project addresses these questions through data analysis and interactive dashboard visualisation.

## 3. Project Objectives

- Calculate total customers, churned customers and retained customers.
- Measure overall customer churn and retention rates.
- Identify customer segments with higher churn rates.
- Analyse churn patterns across contract types, internet services and payment methods.
- Examine the relationship between customer tenure and churn.
- Explore how technical support subscription relates to customer retention.
- Develop an interactive Power BI dashboard.
- Provide actionable business recommendations to support customer retention.

## 4. Dataset Overview

**Dataset:** Telco Customer Churn

| Description | Details |
|---|---|
| Total Records | 7,043 |
| Total Columns | 21 |
| Data Format | CSV |
| Unit of Analysis | Individual Customer |
| Target Variable | Churn |

### Important Features

- Customer_ID – Unique customer identifier
- Gender – Customer gender
- Senior_Citizen – Senior citizen status
- Tenure – Number of months the customer has stayed
- Contract – Customer contract type
- Internet_Service – Type of internet service
- Tech_Support – Technical support subscription status
- Payment_Method – Customer payment method
- Monthly_Charges – Monthly subscription charges
- Total_Charges – Total recorded customer charges
- Churn – Whether the customer left the company

## 5. Tools and Technologies

| Tool | Purpose |
|---|---|
| Microsoft Excel | Initial data inspection |
| Power Query | Data cleaning and transformation |
| Power BI | Interactive dashboard development |
| DAX | KPI calculations and measures |

## 6. Data Cleaning and Preparation

Data cleaning and preparation were performed using Excel Power Query.

The following activities were completed:

1. Imported the CSV dataset into Power Query.
2. Reviewed column names and data types.
3. Checked for duplicate Customer_ID values.
4. Identified missing values in the dataset.
5. Investigated 11 missing values in Total_Charges.
6. Replaced the 11 missing Total_Charges values with 0 because the corresponding customers had zero tenure and had not churned.
7. Checked categorical values for inconsistencies.
8. Reviewed column quality, distribution and data profiling.
9. Loaded the cleaned dataset into Power BI.

All 7,043 customer records were retained after data preparation.

## 7. Key Performance Indicators (KPIs)

The following KPIs were developed using DAX in Power BI.

| KPI | Result |
|---|---:|
| Total Customers | 7,043 |
| Churned Customers | 1,869 |
| Retained Customers | 5,174 |
| Churn Rate | 26.54% |
| Retention Rate | 73.46% |

### Business Interpretation

The overall churn rate is 26.54%, meaning approximately one in four customers discontinued their services.

Although 73.46% of customers were retained, the churn rate indicates an opportunity for the company to improve customer retention.

## 8. Power BI Dashboard

The interactive dashboard includes five KPI cards, four slicers and six visualisations.

### Dashboard Preview

![Telco Customer Churn Analysis Dashboard](Screenshots/Dashboard.png)

### Interactive Filters

- Contract
- Internet Service
- Gender
- Payment Method

These slicers allow users to explore churn patterns across different customer segments.

## 9. Key Findings and Business Insights

### 9.1 Churn Rate by Contract Type

| Contract Type | Churn Rate |
|---|---:|
| Month-to-month | 42.71% |
| One year | 11.27% |
| Two year | 2.83% |

**Insight:** Month-to-month customers have the highest churn rate, while two-year contract customers have the lowest.

**Business Recommendation:** Introduce attractive long-term contract offers, loyalty benefits and renewal incentives to encourage customers to maintain their subscriptions.

### 9.2 Churn Rate by Internet Service

| Internet Service | Churn Rate |
|---|---:|
| Fiber optic | 41.89% |
| DSL | 18.96% |
| No internet service | 7.40% |

**Insight:** Fiber optic customers show the highest churn rate among the internet service categories.

**Business Recommendation:** Investigate service quality, pricing, customer complaints and support experience among fiber optic subscribers.

### 9.3 Churn Rate by Technical Support

The dashboard indicates approximately:

- No technical support: 41%
- Technical support: 16%
- No internet service: 8%

**Insight:** Customers without technical support have a considerably higher churn rate than customers with technical support.

**Business Recommendation:** Improve technical assistance, provide proactive troubleshooting and make support services more accessible.

### 9.4 Churn Rate by Payment Method

Approximate values from the dashboard:

| Payment Method | Churn Rate |
|---|---:|
| Electronic check | 45% |
| Mailed check | 19% |
| Bank transfer (automatic) | 17% |
| Credit card (automatic) | 15% |

**Insight:** Electronic check users show the highest churn rate compared with customers using other payment methods.

**Business Recommendation:** Review the billing experience and encourage convenient automatic payment options.

### 9.5 Churn Rate by Customer Tenure

**Insight:** The visualisation shows a general downward trend in churn rate as customer tenure increases. Customers with shorter tenure generally demonstrate higher churn rates.

**Business Recommendation:** Strengthen customer onboarding, provide early engagement and resolve service issues quickly to improve retention during the initial months.

### 9.6 Total Customer Charges by Churn Status

| Churn Status | Total Charges | Share |
|---|---:|---:|
| Retained (No) | 13.19M | 82.17% |
| Churned (Yes) | 2.86M | 17.83% |

**Insight:** Retained customers account for the majority of total recorded customer charges.

**Business Recommendation:** Monitor customer attrition and identify opportunities to retain customers who may discontinue their subscriptions.

*Note: Total Charges represents cumulative customer-level charges in this dataset, not monthly revenue or revenue lost during a specific period.*

## 10. Overall Business Recommendations

Based on the analysis, the following strategies could help improve customer retention:

1. **Contract Retention:** Encourage month-to-month customers to consider longer-term contracts through loyalty benefits and attractive offers.
2. **Early Customer Engagement:** Improve onboarding and provide additional support during the initial months.
3. **Service Quality:** Investigate customer dissatisfaction among fiber optic subscribers.
4. **Technical Support:** Improve support accessibility and proactive troubleshooting.
5. **Payment Convenience:** Review the electronic check payment experience and promote convenient payment alternatives.
6. **Continuous Monitoring:** Track churn rates across customer segments to evaluate retention performance.

## 11. Project Limitations

- The analysis is based on historical customer data and does not predict future churn.
- The dataset does not provide confirmed reasons for customer cancellation.
- Observed relationships indicate associations and do not establish causation.
- Some chart values are approximate readings from the dashboard.
- Total_Charges is cumulative customer-level data rather than period-based revenue.

## 12. Future Enhancements

1. **Predictive Churn Modelling:** Develop machine learning models to identify customers who are more likely to leave.
2. **Customer Segmentation:** Group customers based on tenure, service usage, billing behaviour and contract preferences.
3. **Advanced Revenue Analysis:** Investigate the financial impact of customer churn using period-based revenue measures.
4. **Automated Reporting:** Develop automated dashboards to monitor churn and retention KPIs.
5. **Customer Feedback Analysis:** Incorporate customer complaints and cancellation reasons to better understand the underlying causes of churn.

## 13. Conclusion

This project analysed 7,043 telecommunications customer records and identified an overall churn rate of 26.54%.

The analysis highlighted higher churn rates among month-to-month contract customers, fiber optic subscribers, customers without technical support and electronic check users. It also revealed a general decline in churn as customer tenure increases.

By combining Excel, Power Query and Power BI, this project demonstrates how data cleaning, KPI development and interactive visualisation can transform raw customer data into meaningful business insights.

The findings provide a foundation for identifying high-risk customer segments and developing data-driven customer retention strategies.

---

**Project Category:** Customer Analytics | Churn Analysis | Business Intelligence

**Skills Demonstrated:** Data Cleaning | Data Transformation | Power Query | DAX | KPI Development | Data Visualisation | Exploratory Data Analysis | Business Interpretation | Dashboard Development

---

👩‍💻 Author Maathangi

Data Analyst | Microsoft Excel | SQL | Power BI | Python

🔗 GitHub: https://github.com/Maathangi1412

🔗 LinkedIn: www.linkedin.com/in/maathangip
