# Food Delivery Platform Performance Analysis

## About This Project

I built this project in Excel to analyze the performance of a food delivery platform using data from 2024 and 2025.

I started with the raw dataset and worked through the analysis step by step. First, I checked the data and created a few validation checks. Then I used Power Query, PivotTables, formulas, and charts to look at sales, orders, cities, delivery performance, promotions, customer satisfaction, weekends, and festivals.

The final part of the project was creating a dashboard and turning the analysis into some business observations and recommendations.

---

## What I Wanted to Find

While working on the project, I mainly wanted to answer questions like:

* Is the business growing from 2024 to 2025?
* Which cities are doing better?
* Which restaurants, cuisines, and categories perform well?
* Are deliveries usually early, on time, or late?
* Do promotions actually make a noticeable difference?
* What happens to customer satisfaction at different ratings?
* How much business comes from weekends?
* How much business comes from festivals?

---

## Dataset

The dataset contains food delivery records for **2024 and 2025**.

Some of the main columns are:

* Date
* Restaurant
* City
* Cuisine Type
* Category
* Weather
* Rating
* Customer Satisfaction
* Orders
* Sales
* Commission
* Net Sales
* Delivery Time
* Promotion
* Weekend
* Festival

The cities included are:

**Bangalore, Chennai, Delhi, Hyderabad, Mumbai, and Pune.**

---

## Tools I Used

* Microsoft Excel
* Power Query
* PivotTables
* PivotCharts
* Excel formulas

---

## Data Quality Checks

Before starting the main analysis, I checked whether the data was consistent enough to use.

Some of the checks I performed were:

* Checked the date range
* Checked numeric columns
* Checked the 0/1 fields
* Checked delivery times
* Calculated delivery delay
* Checked Net Sales
* Checked Commission
* Checked promotion, weekend, and festival fields

The dataset covers:

**01-Jan-2024 to 31-Dec-2025**

I also checked Net Sales using:

**Net Sales = Sales - Commission**

The overall totals I got were:

| KPI              |          Value |
| ---------------- | -------------: |
| Total Orders     |     32,099,435 |
| Total Sales      | ₹9,557,012,837 |
| Total Commission | ₹1,778,007,160 |
| Total Net Sales  | ₹7,778,562,143 |

For delivery performance, I created:

**Delivery Delay = Delivery Time Actual - Delivery Time Minimum**

The delay values were roughly between **-5 and +5 minutes**.

I also created a delivery status column to classify records as:

* Early
* On Time
* Late

One thing I noticed was that `Is_Peak_Hour` contained only `0`, so there wasn't enough variation to make a useful peak-hour comparison.

---

## Analysis I Performed

I looked at the data from different angles:

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

After completing the analysis, I created an Excel dashboard with the main KPIs and charts.

### KPIs

* Total Orders
* Total Sales
* Total Commission
* Total Net Sales

### Charts

* Monthly Sales Trend — 2024 vs 2025
* Sales by City
* Delivery Performance
* Promo vs Non-Promo Performance
* Orders by Customer Rating

The idea was to keep the dashboard simple enough that someone could look at it and understand the main business numbers quickly.

---

## Some Findings From My Analysis

### Business Growth

When I compared 2024 with 2025:

* Orders increased by approximately **7.04%**
* Sales increased by approximately **7.06%**

So the business was growing in both orders and sales.

### City Performance

Mumbai had the highest sales at approximately **₹1.68 billion**.

Bangalore had the highest number of orders at approximately **6.72 million**.

This was one of the interesting things I found because the city with the highest orders was not the city with the highest sales.

### Delivery Performance

The average delivery delay was approximately **0 minutes**.

The delay values were roughly between **-5 and +5 minutes**, so the actual delivery time was generally close to the expected delivery time in this dataset.

### Promotion Performance

I compared promotional and non-promotional orders.

Average Sales per Order:

* Non-Promo: **₹297.76**
* Promo: **₹297.55**

Average Net Sales per Order:

* Non-Promo: **₹242.34**
* Promo: **₹242.21**

The difference was very small.

So from the data I had, I couldn't see a major difference in average order value between promo and non-promo orders.

But I would **not** say that promotions are useless. The dataset doesn't contain enough information about discount costs and incremental customers to properly calculate promotion ROI.

### Customer Satisfaction

For the records with a **4.7 rating**, the average customer satisfaction was approximately **0.610**.

For the records with a **3.8 rating**, it was approximately **0.556**.

Higher-rated records had higher average satisfaction, but that didn't automatically mean they had higher sales or more orders.

### Weekend Performance

Weekdays:

* Orders: **23,005,799**
* Sales: **₹6,849,528,311**

Weekends:

* Orders: **9,093,636**
* Sales: **₹2,707,484,526**

So most of the business activity happened during weekdays.

### Festival Performance

Non-festival periods:

* Orders: **30,709,104**
* Sales: **₹9,143,082,625**

Festival periods:

* Orders: **1,390,331**
* Sales: **₹413,930,212**

Festival periods made up a relatively small part of the overall business in this dataset.

---

## What I Would Recommend

Based on what I found, I would focus on a few areas.

**1. Look at cities differently**

Mumbai is strong in sales, while Bangalore is strong in order volume. So I wouldn't use exactly the same strategy for every city.

**2. Keep monitoring delivery performance**

Delivery performance was close to the expected time in the data. Maintaining that as order volume grows would be important.

**3. Measure promotions properly**

The average order values were almost the same for promo and non-promo orders. To understand whether promotions are actually worth the money, I would want to see discount cost, promotion cost, new customers, repeat orders, and incremental revenue.

**4. Look for ways to increase weekend demand**

Weekdays contribute most of the business. That makes weekends an area where targeted campaigns could be tested.

**5. Use festivals selectively**

Festival periods are a smaller part of the overall business, so I would measure individual festival campaigns instead of assuming every festival campaign will work.

---

## Limitations I Found

There were also some things I could not properly answer with this dataset.

* I couldn't calculate actual promotion ROI because promotion and discount costs were not available.
* Net Sales is not the same as profit because other operating expenses were not included.
* There wasn't enough customer-level information to analyze customer retention, churn, or lifetime value.
* The analysis shows patterns in the data, but it does not prove that one factor caused another.
* `Is_Peak_Hour` contained only `0`, so I couldn't compare peak and non-peak hours properly.

I think mentioning these limitations is important because it shows what the data can and cannot actually tell us.

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

### Folders

**Data** — Raw dataset and data-related files

**Analysis** — Excel workbook containing the analysis

**Documentation** — Detailed project documentation

**Screenshots** — Screenshots from the analysis and dashboard

**Dashboard** — Final dashboard output

---

## What I Practiced Through This Project

This project gave me practical experience with:

* Excel
* Power Query
* Data cleaning
* Data quality checks
* PivotTables
* PivotCharts
* Calculations
* KPI analysis
* Year-over-year comparison
* Business analysis
* Dashboard creation
* Finding insights from data
* Turning findings into recommendations

The biggest thing I learned was that analysis is not just about getting a number. The important part is understanding **what the number means and whether it is actually useful for the business.**

---

## Conclusion

This project started with a large raw dataset and ended with a structured Excel analysis and dashboard.

The analysis showed positive growth from 2024 to 2025, different performance across cities, relatively stable delivery timing, very similar average order values between promotional and non-promotional orders, and different demand patterns between weekdays, weekends, and festivals.

There are also areas where the available data wasn't enough to give a complete answer, especially promotion ROI and profitability.

Overall, this project helped me practice the complete process:

**Raw Data → Data Quality → Analysis → Dashboard → Findings → Recommendations**

---

**Project:** Food Delivery Platform Performance Analysis
