# Customer Lifetime Value Analysis and Future Spending Prediction

# Project Overview

This project analyzes customer behavior and customer lifetime value (CLV) to identify high-value customers and predict future customer spending.

The objective is to help businesses improve customer retention, optimize marketing strategies, and increase long-term revenue through data-driven customer analysis.

---

# Business Problem

Customer Lifetime Value (CLV) represents the total value a customer is expected to generate for a business over time.

Businesses focus on increasing CLV because:
- Existing customers are more cost-effective than acquiring new customers
- Loyal customers generate repeat revenue
- Long-term customer relationships improve profitability

This project aims to:
- Understand customer value
- Segment customers based on spending behavior
- Predict future customer spending
- Recommend strategies to improve long-term customer value

---

# Dataset Description

The dataset contains customer demographic, engagement, and spending behavior information.

## Important Columns
- CustomerID
- Age
- AnnualIncome
- WebsiteVisits
- AppSessions
- PreviousOrders
- AverageOrderValue
- DaysSinceLastPurchase
- ReturnRate
- CancellationRate
- LoyaltyTier
- DiscountUsedLastCampaign
- Year1Spending
- FutureSpending

---

# Tools and Libraries Used

## Tools
- VS Code
- Jupyter Notebook
- GitHub

## Python Libraries
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

---

# Data Cleaning and Feature Engineering Summary

The following preprocessing and feature engineering steps were performed:
- Filled missing AnnualIncome values using median imputation
- Filled missing AverageOrderValue values using median imputation
- Created EngagementScore feature
- Created SpendingPerOrder feature
- Performed outlier analysis
- Encoded categorical variables
- Standardized numerical features

## Feature Descriptions

### EngagementScore
Measures customer engagement using website visits and app sessions.

### SpendingPerOrder
Represents average customer spending efficiency per order.

---

# Exploratory Data Analysis

EDA included:
- Distribution of future spending
- Relationship between income and future spending
- Relationship between website visits and future spending
- Relationship between previous spending and future spending
- Correlation heatmap
- Outlier analysis

## Key Insights
- Previous spending strongly influences future spending.
- Higher engagement customers tend to spend more.
- Income and order behavior positively affect customer value.
- High-value customers contribute significantly to future revenue.

---

# Customer Segmentation Summary

Customers were segmented using K-Means clustering into:
- High-value customers
- Medium-value customers
- Low-engagement customers

## Segmentation Logic
Segmentation was based on:
- Previous spending
- Future spending
- Engagement score

---

# Regression Model Summary

Two regression models were trained:
- Linear Regression
- Decision Tree Regressor

The objective was to predict future customer spending.

---

# Model Evaluation Results

| Model | MAE | RMSE | R² Score |
|---|---|---|---|
| Linear Regression | 956.26 | 1220.62 | 0.93 |
| Decision Tree | 1226.81 | 1534.23 | 0.89 |

## Model Selection
Linear Regression performed better overall with:
- Lower prediction error
- Higher R² score
- Better future spending prediction capability

---

# Final LTV Growth Strategy

- Provide premium offers for high-value customers.
- Use upselling campaigns for medium-value customers.
- Re-engage low-engagement customers using discounts and personalized offers.
- Improve customer engagement through loyalty programs and personalized recommendations.
- Focus retention strategies on customers with strong historical spending patterns.
- Reduce cancellation and return rates to improve long-term profitability.

---

# Project Outputs

The repository contains:
- notebook.ipynb
- requirements.txt
- dataset_source.md
- outputs/customer_segments.csv
- outputs/model_results.csv
- README.md

---

# How to Run the Project

## Clone Repository
```bash
git clone https://github.com/Sathvikaaaaaa/Customer-lifetime-value-analysis.git