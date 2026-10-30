# 📊 Customer Churn Analysis Dashboard – SaiKet Systems

## 📌 Project Overview

The Customer Churn Analysis Dashboard is an interactive Business Intelligence project developed using Microsoft Power BI as part of the SaiKet Systems internship.

The project focuses on analyzing customer churn behavior, understanding customer segments, and identifying patterns that may contribute to customer attrition.

The dashboard transforms customer data into meaningful visual insights through KPIs, DAX measures, and interactive charts.

## 🎯 Project Objectives

- Analyze overall customer data and churn behavior.
- Calculate important business KPIs.
- Identify churn patterns across different contract types.
- Understand churn distribution by gender.
- Analyze customer churn based on internet service.
- Explore payment method preferences among churned customers.
- Examine Streaming TV and Streaming Movies usage patterns.
- Present business insights through an interactive dashboard.

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Microsoft Power BI Desktop | Dashboard Development |
| DAX | KPI and Measure Calculations |
| Power BI Visualizations | Data Presentation |
| CSV Dataset | Customer Data Source |

## 📂 Dataset Description

**Dataset:** Telco Customer Churn Dataset

The dataset contains customer-related information, including:

- Customer ID
- Gender
- Contract
- Internet Service
- Payment Method
- Monthly Charges
- Total Charges
- Tenure
- Streaming Movies
- Streaming TV
- Churn Status

## 📈 Key Performance Indicators (KPIs)

The dashboard includes four major KPIs:

1. **Total Customers** – Displays the customer count.
2. **Churned Customers** – Displays the number of customers who discontinued the service.
3. **Churn Rate** – Measures the percentage of customers who churned.
4. **Average Monthly Charges** – Shows the average monthly customer charges.

## 📊 Dashboard Visualizations

### 1. Churned Customers by Contract
Analyzes customer churn across Month-to-month, One year, and Two year contract categories.

### 2. Churned Customers by Gender
Compares churn distribution between male and female customers.

### 3. Churned Customers by Internet Service
Analyzes churn patterns across Fiber Optic, DSL, and No Internet Service categories.

### 4. Churned Customers by Payment Method
Uses a donut chart to visualize churn distribution across different payment methods.

### 5. Streaming Movies and Streaming TV Analysis
Explores customer streaming service usage patterns and their relationship with churn.

## 🧮 DAX Measures

### Churned Customers

```dax
Churned Customers =
CALCULATE(
    COUNTROWS('Telco_Customer_Churn_Dataset'),
    'Telco_Customer_Churn_Dataset'[Churn] = "Yes"
)
```

### Churn Rate

```dax
Churn Rate =
DIVIDE(
    [Churned Customers],
    COUNTROWS('Telco_Customer_Churn_Dataset')
)
```

### Average Monthly Charges

```dax
Average Monthly Charges =
AVERAGE(
    'Telco_Customer_Churn_Dataset'[MonthlyCharges]
)
```

## 🔍 Key Insights

- Month-to-month contract customers show the highest churn count.
- Fiber Optic customers represent the largest churn group among internet service categories.
- Electronic Check is the most prominent payment method in the churn distribution.
- Gender-based analysis helps compare customer churn across segments.
- Streaming service analysis provides additional understanding of customer behavior.

## 📁 Project Structure

```text
SaiKet_Customer_Churn_Analysis/
│
├── data/
│   └── Telco_Customer_Churn_Dataset.csv
│
├── dashboard/
│   └── SaiKet_Customer_Churn_Analysis.pbix
│
├── screenshots/
│   └── Dashboard_Screenshot.png
│
├── documentation/
│   └── README.md
│
└── reports/
```

## 🚀 Project Outcome

Successfully developed an interactive Power BI dashboard to analyze customer churn, monitor key business performance indicators, and identify customer segments with higher churn.

This project demonstrates practical skills in:

- Data Analysis
- Business Intelligence
- Power BI Dashboard Development
- DAX Calculations
- KPI Development
- Data Visualization
- Business Insight Generation

## 👨‍💻 Author

**Sebastin Naveen Kumar**

- **Organization:** SaiKet Systems
- **Internship Task:** Interactive Dashboard
- **Project Domain:** Data Analytics & Business Intelligence

---

⭐ This project was developed as part of the SaiKet Systems Internship Program.