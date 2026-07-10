## Tableau Dashboards Portfolio

A collection of 2 interactive Tableau dashboards covering road safety analytics and consumer complaint analysis. Each is a single-page dashboard built with calculated fields, filters, and Tableau's native visuals (maps, donut charts, heatmaps, and KPI cards).

| # | Dashboard | File | Domain |
|---|-----------|------|--------|
| 1 | [Road Accident Dashboard](#1-road-accident-dashboard) | `Road_Accident_Dashboard.twbx` | Public Safety / Transportation Analytics |
| 2 | [Credit Card Complaints Dashboard](#2-credit-card-complaints-dashboard) | `Credit_Card_Complaints_Dashboard.twbx` | Finance / Customer Complaints Analytics |

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

## Tools used
- Tableau Desktop
- Calculated fields (YoY % change, rate/ratio measures, dynamic date parameters)
- Tableau Prep / data source cleanup
- Filters, parameters, and dashboard actions for interactivity

## Repository structure
```
├── Road_Accident_Dashboard.twbx
├── Credit_Card_Complaints_Dashboard.twbx
└── README.md
```

## How to use
1. Download/clone the repo.
2. Open the `.twbx` file in Tableau Desktop or Tableau Reader (free download from Tableau).
3. Use the filter panel on each dashboard to slice by year, severity, company, or state.
4. Hover over any visual for tooltips with exact values; click map points or bars to cross-filter the dashboard.
