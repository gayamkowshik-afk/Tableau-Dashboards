## Tableau Dashboards Portfolio

A collection of 4 interactive Tableau dashboards covering road safety analytics, consumer complaint analysis, bank loan performance, and pizza sales analytics. Each is a single-page (or multi-tab) dashboard built with calculated fields, filters, and Tableau's native visuals (maps, donut charts, heatmaps, and KPI cards).

| # | Dashboard | File | Domain |
|---|-----------|------|--------|
| 1 | [Road Accident Dashboard](#1-road-accident-dashboard) | `Road_Accident_Dashboard.twbx` | Public Safety / Transportation Analytics |
| 2 | [Credit Card Complaints Dashboard](#2-credit-card-complaints-dashboard) | `Credit_Card_Complaints_Dashboard.twbx` | Finance / Customer Complaints Analytics |
| 3 | [Bank Loan Report Dashboard](#3-bank-loan-report-dashboard) | `Bank_Loan_Report_Dashboard.twbx` | Finance / Lending Analytics |
| 4 | [Pizza Sales Dashboard](#4-pizza-sales-dashboard) | `Pizza_Sales_Dashboard.twbx` | Retail / F&B Sales Analytics |

---

## 1. Road Accident Dashboard

A UK road safety report comparing accident and casualty trends year-over-year, with a drill-down into serious casualties by vehicle type, weather, road surface, road type, and location.

**Filters:** Current Year (2022), Previous Year (2021), Select Accident Severity (Serious)

**KPI cards (with monthly trend sparkline, YoY % change)**
- Total Accidents: 1,44,419 ▼11.70%
- Total Casualties: 1,95,737 ▼11.89%
- Fatal Casualties: 2,855 ▼26.40%
- Serious Casualties: 27,045 ▼16.30%
- Slight Casualties: 1,65,837 ▼10.82%

**Visuals**
- **Serious Casualties by Vehicle Type** (icon cards) — Agricultural Vehicle 61 (▼39.60%), Bus/Coach 912 (▲1.67%), Car 21,469 (▼16.60%), Bicycle 2,164 (▼17.94%), Motorcycle 241 (▼20.72%), Van/Goods Vehicle 2,198 (▼16.46%)
- **Serious Casualties by Weather Condition** (donut) — Fine 83.73%, Rain 10.54%, Others 3.54%, Snow/Fog 2.19%
- **Serious Casualties by Road Surface** (donut) — Dry 69.62%, Wet 24.76%, Frost/Snow 5.54%, Unknown 0.08%
- **Serious Casualties by Road Type** (bar) — Single carriageway 78.52%, Dual carriageway 14.99%, Roundabout 3.74%, One way street 1.55%, Slip road 0.89%, Null 0.31%
- **Serious Casualties by Location** (map) — geo-plotted incident points across the UK (England, Scotland, Wales)

**Key insight:** Cars account for the vast majority of serious casualties (21,469), and most serious accidents occur in fine weather on dry, single-carriageway roads — pointing to driver behavior and road design as bigger contributing factors than adverse conditions. Nearly all categories improved year-over-year, led by a 26.40% drop in fatal casualties.

---

## 2. Credit Card Complaints Dashboard

A consumer complaints tracker monitoring intake volume, resolution speed, and company response quality across states, issue types, and submission channels.

**Filters:** Year of Date Received, Company, State
**Export options:** PDF, Image, PowerPoint

**KPI cards (with trend sparkline)**
- Total Complaints: 86,893 (Rolling 12 months: 20,202)
- Timely Response: 85,934 — Closed %: 98.9%
- In Progress Complaints: 329 — In Progress %: 0.38%

**Visuals**
- **Weekly Trend** (area chart, toggle to Daily/Monthly) — complaint volume 2016–2021, average line at 310.33/week, with a spike around 2016 and a steady climb through 2020–2021
- **State Wise Complaints** (filled map) — California leads with 12,102, followed by Texas 5,625, New York 1,906, Georgia 2,914, Illinois 3,240, Kentucky 2,579, Massachusetts 2,250
- **Top Issue** (bar) — Billing disputes (highest), Other, Identity theft/Fraud, Closing/Cancelling account, APR or interest rate, Late fee, Customer service, Delinquent account, Credit determination, Advertising and marketing
- **Company Response** (table) — Closed with explanation 51,873 (59.92%), Closed with monetary relief 17,942 (20.73%), Closed with non-monetary relief 9,215 (10.65%), Closed without relief 4,246 (4.91%), Closed with relief 2,500 (2.89%), Closed 649 (0.75%), Untimely response 139 (0.16%)
- **Daily Complaints** (calendar heatmap) — day-by-day intensity view for a selected month (e.g., December 2016)
- **Submitted Via** (breakdown) — Web 68.92%, Referral 16.58%, Phone 7.48%, Postal mail 5.96%, Fax 1.00%, Email 0.05%

**Key insight:** Billing disputes are the top driver of complaints, nearly 99% of cases receive a timely response, and the Web is by far the dominant submission channel (68.92%) — with the majority of complaints (59.92%) resolved simply through explanation rather than monetary relief.

---

## 3. Bank Loan Report Dashboard

A three-page lending performance report tracking loan application volume, funding, repayment quality, and borrower demographics, with a page dedicated to good vs. bad loan segmentation and a full transaction-level detail grid.

**Filters:** Verification Status, Grade, Purpose

**KPI cards (with MTD and MoM % change, shown on every page)**
- Total Loan Applications: 38.6K (MTD 4.3K, MoM ▲6.9%)
- Total Funded Amount: $435.8M (MTD $54.0M, MoM ▲13.0%)
- Total Amount Received: $473.1M (MTD $58.1M, MoM ▲15.8%)
- Avg Interest Rate: 12.0% (MTD 13.7%, MoM ▲2.7%)
- Avg DTI: 13.3% (MTD 12.4%, MoM ▲3.5%)

### Page 1 — Summary
- **Good Loan Issued** (donut, 86.2%) — Good Loan Applications 33.2K, Good Loan Funded Amount $370.2M, Good Loan Amount Received $435.8M
- **Bad Loan Issued** (donut, 13.8%) — Bad Loan Applications 5.3K, Bad Loan Funded Amount $65.5M, Bad Loan Amount Received $37.3M
- **Loan Status** (table) — breakdown by Charged Off, Current, and Fully Paid across Total Loan Applications, Total Funded Amount, Total Amount Received, MTD Funded/Received Amount, Avg Interest Rate, and Avg DTI

### Page 2 — Overview
- **Total Loan Applications by Month** (line chart) — steady upward trend from ~2K in January to ~4K in December
- **Total Loan Applications by State** (filled map) — California and Texas as leading states
- **Total Loan Applications by Term** (donut) — 36 months 73.20%, 60 months 26.80%
- **Total Loan Applications by Employee Length** (bar) — 10+ years 8.9K, <1 year 4.6K, 2 years 4.4K, 3 years 4.1K, down to 9 years 1.3K
- **Total Loan Applications by Purpose** (bar) — Debt consolidation 18.2K (dominant), credit card 5.0K, other 2.9K, home improvement 2.9K, major purchase, small business, car, wedding, medical, moving, house, vacation, educational, renewable_energy
- **Total Loan Applications by Home Ownership** (treemap) — RENT 18.4K, MORTGAGE 17.2K, OWN 2.8K

### Page 3 — Details
- **Loan-level data grid** — Id, Purpose, Home Ownership, Grade, Sub Grade, Issue Date, Loan Amount, Int Rate, Installment, and Total Payment for full drill-down/audit-level inspection of every loan record

**Key insight:** 86.2% of issued loans are performing well ("Good Loan"), with debt consolidation as the overwhelming top purpose (18.2K applications) and RENT/MORTGAGE borrowers making up nearly 92% of all applications — signalling where underwriting and collections effort is best concentrated.

---

## 4. Pizza Sales Dashboard

A two-page retail sales dashboard for a full year of pizza order data (2015), covering revenue performance, best/worst sellers, order timing patterns, and category/size mix.

**Filters:** Pizza Category, Order Date (01-01-2015 to 31-12-2015, slider range)

**KPI cards (shown on every page)**
- Total Revenue: $817.9K
- Avg Order Value: 38.31
- Total Pizzas Sold: 49.6K
- Total Orders: 21.4K
- Avg Pizzas per Order: 2.32

### Page 1 — Home
- **Top 5 Pizzas by Revenue** — Thai Chicken $43.4K, Barbecue Chicken $42.8K, California Chicken $41.4K, Classic Deluxe $38.2K, Spicy Italian $34.8K
- **Top 5 Pizzas by Total Pizzas Sold** — Classic Deluxe 2.5K, Barbecue Chicken 2.4K, Hawaiian 2.4K, Pepperoni 2.4K, Thai Chicken 2.4K
- **Top 5 Pizzas by Total Orders** — Classic Deluxe 2.3K, Hawaiian 2.3K, Pepperoni 2.3K, Barbecue Chicken 2.3K, Thai Chicken 2.2K
- **Bottom 5 Pizzas by Revenue** — Brie Carre $11.6K, Green Garden $14.0K, Spinach Supreme $15.3K, Mediterranean $15.4K, Spinach Pesto $15.6K
- **Bottom 5 Pizzas by Total Pizzas Sold** — Brie Carre 0.5K, Mediterranean 0.9K, Calabrese 0.9K, Spinach Supreme 1.0K, Soppressata 1.0K
- **Bottom 5 Pizzas by Total Orders** — Brie Carre 0.5K, Mediterranean 0.9K, Calabrese 0.9K, Spinach Supreme 0.9K, Chicken Pesto 0.9K
- Sidebar call-outs on busiest hours/weeks and top revenue/quantity/order contributors (Thai Chicken, Classic Deluxe, Brie Carre)

### Page 2 — Best/Worst Sellers
- **Hourly Trend for Total Pizzas** (stacked bar by category) — two clear peaks, 12–1 PM and 4–7 PM, with Chicken and Classic categories leading most hours
- **Weekly Trend for Total Orders** (line) — average 402.8 orders/week, peaking at 491 in week 48 (December) and dipping to a low of 171 in week 1
- **% of Sales by Pizza Category** (donut) — Classic $220.1K (26.91%), Supreme $208.2K (25.46%), Chicken $195.9K (23.96%), Veggie $193.7K (23.68%)
- **% of Sales by Pizza Size** (bar) — Large leads, followed by Medium, Small, with X-Large and XX-Large negligible
- **Total Orders & Pizzas Sold by Pizza Category** (bar) — Classic 14,888 pizzas / 10,859 orders, Supreme 11,987 / 9,085, Veggie 11,649 / 8,941, Chicken 11,050 / 8,536

**Key insight:** The Classic category drives the most sales, orders, and pizzas sold, and Large is by far the preferred size. Order volume peaks around lunch (12–1 PM) and dinner (4–7 PM), with the year's single busiest week landing in week 48 (late November/early December) — useful signal for staffing and inventory planning.

---

## Tools used
- Tableau Desktop
- Calculated fields (YoY % change, MoM % change, rate/ratio measures, dynamic date parameters)
- Tableau Prep / data source cleanup
- Filters, parameters, and dashboard actions for interactivity
- Multi-page/tabbed dashboard navigation (Bank Loan Report, Pizza Sales)

## Repository structure
```
├── Road_Accident_Dashboard.twbx
├── Credit_Card_Complaints_Dashboard.twbx
├── Bank_Loan_Report_Dashboard.twbx
├── Pizza_Sales_Dashboard.twbx
└── README.md
```

## How to use
1. Download/clone the repo.
2. Open the `.twbx` file in Tableau Desktop or Tableau Reader (free download from Tableau).
3. Use the filter panel on each dashboard to slice by year, severity, company, state, loan grade/purpose, or pizza category/date.
4. Hover over any visual for tooltips with exact values; click map points, bars, or table rows to cross-filter the dashboard.
