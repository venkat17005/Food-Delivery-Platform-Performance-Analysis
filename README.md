# Food Delivery Platform Performance Analysis

## Project Overview

This project analyzes food delivery platform performance using Microsoft Excel.

The main goal was to take raw food delivery business data, perform data quality checks, analyze important business metrics, and build a dashboard that can help understand sales, orders, delivery performance, customer satisfaction, promotions, and location-level performance.

The project follows a practical Data Analyst workflow:

**Raw Data → Data Quality Check → Analysis → Dashboard → Insights → Recommendations**

---

## Business Problem

A food delivery platform generates a large amount of business data, but raw data alone does not show where the business is performing well or where improvements are needed.

This analysis focuses on questions such as:

* How are orders and sales changing over time?
* Is the business growing year over year?
* Which cities generate the most orders and sales?
* How well are deliveries performing?
* Do promotional and non-promotional orders differ in value?
* What is the relationship between customer ratings and satisfaction?
* How does business performance differ between weekdays and weekends?
* How much business comes from festival periods?
* What areas could be considered for future improvement?

---

## Project Objective

The main objective of this project is to analyze food delivery platform performance and identify opportunities to improve:

* Sales growth
* Order performance
* Delivery operations
* Customer experience
* Promotional effectiveness
* Location-level performance

The project also demonstrates how Excel can be used to follow a complete Data Analyst workflow from raw data to business recommendations.

---

## Dataset

The dataset contains food delivery business data for **2024 and 2025**.

The data includes information related to:

* Date and time period
* Restaurants
* Cities
* Cuisine types
* Restaurant categories
* Weather
* Customer ratings
* Customer satisfaction
* Orders
* Sales
* Commission
* Net Sales
* Delivery times
* Promotions
* Weekends
* Festivals
* Packaging charges

### Cities included

* Bangalore
* Chennai
* Delhi
* Hyderabad
* Mumbai
* Pune

---

## Tools Used

* **Microsoft Excel**
* **Power Query**
* **PivotTables**
* **PivotCharts**
* **Excel formulas**
* **Data quality checks**
* **Dashboard creation**

---

## Data Quality Checks

Before starting the analysis, the data was checked for consistency and validity.

The checks included:

* Date range validation
* City validation
* Numeric field validation
* Binary field validation
* Delivery time validation
* Delivery delay calculation
* Net Sales consistency
* Commission consistency
* Promotion indicators
* Weekend indicators
* Festival indicators
* Packaging charge indicators
* 24x7 indicators

### Important checks

The dataset covers:

**01-Jan-2024 to 31-Dec-2025**

Net Sales was validated using:

**Net Sales = Sales − Commission**

The overall totals were:

| KPI              |          Value |
| ---------------- | -------------: |
| Total Orders     |     32,099,435 |
| Total Sales      | ₹9,557,012,837 |
| Total Commission | ₹1,778,007,160 |
| Total Net Sales  | ₹7,778,562,143 |

Delivery delay was calculated using:

**Delivery Delay = Delivery Time Actual − Delivery Time Minimum**

The observed delivery delay values ranged approximately from **-5 to +5 minutes**.

---

## Analysis Performed

The analysis covered the following areas:

1. Overall Business Performance
2. Year-over-Year Performance
3. Monthly Performance
4. City Performance
5. Restaurant Performance
6. Cuisine Performance
7. Category Performance
8. Delivery Performance
9. Promotion Performance
10. Customer Performance
11. Weekend Performance
12. Festival Performance

---

## Dashboard

An Excel dashboard was created to provide a quick view of the main business KPIs and performance trends.

### KPI Cards

* Total Orders
* Total Sales
* Total Commission
* Total Net Sales

### Dashboard Charts

* Monthly Sales Trend — 2024 vs 2025
* Sales by City
* Delivery Performance
* Sales: Promo vs Non-Promo
* Orders by Customer Rating

The dashboard was designed to make the analysis easier to understand without having to review every individual PivotTable.

---

## Key Findings

### 1. Year-over-Year Growth

The business showed positive growth from 2024 to 2025.

* Orders increased by approximately **7.04%**
* Sales increased by approximately **7.06%**

This indicates overall growth in both order volume and sales.

### 2. City Performance

**Mumbai generated the highest sales**, at approximately **₹1.68 billion**.

**Bangalore recorded the highest order volume**, with approximately **6.72 million orders**.

This shows that order volume and revenue contribution vary across cities.

### 3. Delivery Performance

The average delivery delay was approximately **0 minutes**.

The observed delay values ranged from approximately **-5 to +5 minutes**.

This indicates that actual delivery times generally stayed close to the expected delivery time in the available data.

### 4. Promotion Performance

Sales per Order was approximately:

* **Non-Promo:** ₹297.76
* **Promo:** ₹297.55

Net Sales per Order was approximately:

* **Non-Promo:** ₹242.34
* **Promo:** ₹242.21

The difference between promotional and non-promotional orders was very small in terms of average order value.

However, promotion effectiveness cannot be fully determined because promotion costs and complete discount information were not available.

### 5. Customer Performance

Records with a **4.7 rating** had an average customer satisfaction score of approximately **0.610**.

Records with a **3.8 rating** had an average customer satisfaction score of approximately **0.556**.

Higher-rated records showed higher average satisfaction, but higher ratings did not automatically correspond to higher sales or order volume.

### 6. Weekend Performance

Weekdays generated:

* **23.01 million orders**
* **₹6.85 billion sales**

Weekends generated:

* **9.09 million orders**
* **₹2.71 billion sales**

Weekend activity represented approximately **28.3% of total orders and sales**.

### 7. Festival Performance

Non-festival periods generated:

* **30.71 million orders**
* **₹9.14 billion sales**

Festival periods generated:

* **1.39 million orders**
* **₹413.93 million sales**

Festival activity represented approximately **4.3% of total orders and sales**.

---

## Business Recommendations

Based on the analysis, the following recommendations can be considered:

### Focus on High-Performing Cities

Mumbai generated the highest sales while Bangalore generated the highest order volume.

Different cities can be approached with different strategies depending on whether the goal is revenue growth or order-volume growth.

### Maintain Delivery Reliability

Delivery performance was close to the expected delivery time in the available data.

The business should continue monitoring delivery performance as order volume grows.

### Evaluate Promotions Based on Actual Impact

Promotional and non-promotional orders showed very similar average order values.

Future promotion analysis should consider:

* Discount amount
* Promotion cost
* Additional orders generated
* New customers acquired
* Customer retention
* Incremental revenue

### Improve Customer Experience

Higher-rated records showed higher customer satisfaction.

Customer experience should continue to be monitored along with other factors such as pricing, restaurant quality, delivery experience, cuisine, and location.

### Use Targeted Weekend Campaigns

Since weekdays contribute the majority of business volume, weekends can be used for targeted campaigns and offers to increase weekend demand.

### Use Festivals as Targeted Opportunities

Festival periods contribute a smaller share of total business volume.

Specific festivals can be used for targeted campaigns, with their incremental impact measured separately.

---

## Project Limitations

There are some limitations to this analysis based on the available data.

### Promotion ROI

Promotion and discount cost information was not available, so true promotion ROI could not be calculated.

### Profitability

Net Sales was calculated as:

**Sales − Commission**

Therefore, Net Sales should not be treated as final company profit because other operating costs were not available.

### Customer-Level Analysis

The dataset does not contain enough customer-level information to perform detailed customer retention, churn, or customer lifetime value analysis.

### Causation

The analysis identifies patterns and relationships in the data.

It does not prove that one factor directly caused a change in another factor.

### Peak Hour Analysis

The `Is_Peak_Hour` field contained only **0** values in the available data, so a meaningful peak-hour versus non-peak-hour comparison could not be performed.

---

## Project Structure

```text
Food-Delivery-Platform-Performance-Analysis/
│
├── Data/
├── Analysis/
├── Documentation/
├── Screenshots/
├── Dashboard/
└── README.md
```

### Folder Purpose

**Data** — Dataset and data-related files

**Analysis** — Completed Excel analysis workbook and analysis outputs

**Documentation** — Detailed project documentation

**Screenshots** — Screenshots of important analysis and dashboard work

**Dashboard** — Final dashboard output

---

## What This Project Demonstrates

This project demonstrates practical skills in:

* Data Cleaning and Validation
* Data Quality Checking
* Power Query
* Excel Formulas
* PivotTables
* PivotCharts
* KPI Analysis
* Year-over-Year Analysis
* Trend Analysis
* Business Performance Analysis
* Data Visualization
* Dashboard Development
* Business Insights
* Data-Driven Recommendations

More importantly, the project focuses on understanding **what the numbers mean for the business**, rather than only calculating metrics.

---

## Conclusion

This project helped transform raw food delivery data into a structured business analysis.

The analysis showed positive year-over-year growth, differences in city-level performance, stable delivery timing, similar average order values between promotional and non-promotional orders, differences in customer satisfaction, and different demand patterns across weekdays, weekends, and festivals.

The final dashboard provides a quick view of the main business KPIs and trends, while the insights and recommendations highlight areas that can be investigated further.

**Overall workflow:**

**Data → Data Quality → Analysis → Visualization → Insights → Recommendations**

---

## Author

**Venkat P.**

**Project:** Food Delivery Platform Performance Analysis
