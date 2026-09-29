# Troy Brown — Power BI & Business Intelligence Portfolio

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/troy-m-brown)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?logo=github)](https://github.com/zero1191)
[![Email](https://img.shields.io/badge/Email-Contact-red?logo=gmail)](mailto:troybrownzero@gmail.com)

---

## 👋 About Me

I'm a Business Intelligence professional with 11+ years at Publix Super Markets, specializing in business intelligence, data visualization, and analytics consulting. Promoted to **Marketing Business Analytics Senior Consultant** in January 2026, I lead advanced analytics and BI initiatives for the Marketing Analytics team — architecting Power BI dashboards, building Alteryx automation workflows, and leveraging Databricks SQL to access and analyze enterprise data that drives marketing decisions.

My work sits at the intersection of **analytics engineering, data storytelling, and strategic consulting** — bridging the gap between technical data infrastructure and business leadership.

**Core stack:** Power BI · Alteryx · Databricks · SQL · Excel · Power Automate · Power Apps

---

## 🛠️ Skills & Technologies

| Category | Tools & Technologies |
|---|---|
| **Visualization** | Power BI (DAX, Power Query, Report Server) |
| **Data Engineering** | Alteryx Designer & Server, Databricks, Apache Spark |
| **Databases & Query** | SQL Server, Spark SQL, Data Modeling, ETL Design |
| **Cloud** | Microsoft Azure (AZ-900 Certified) |
| **Analytics** | Marketing Analytics, Financial Analytics, KPI Development |
| **Collaboration** | Stakeholder Consulting, Cross-functional Teams, Mentoring |

<br>

```
Power BI Desktop     ████████████████████  Expert
Alteryx              ██████████████████░░  Advanced
DAX                  ██████████████████░░  Advanced
Power Query (M)      ████████████████░░░░  Proficient
SQL                  ████████████████░░░░  Proficient
Excel / Power Pivot  ████████████████████  Expert
Power Automate       ██████████████████░░  Advanced
Power Apps           ████████████████░░░░  Proficient
Python (pandas)      ██████████░░░░░░░░░░  Familiar
Azure Data Services  ██████████░░░░░░░░░░  Familiar
```

---

<!-- ============================================================
     FEATURED REPORTS
     ============================================================ -->

## ⭐ Featured Reports

> Click any **Live Report** link to open the interactive Power BI dashboard.

| # | Project | Category | Live Report |
|---|---|---|---|
| 1 | Economic Health Dashboard | Macroeconomic Indicators | [View Report](https://app.powerbi.com/view?r=eyJrIjoiZjUxMDAzOWUtYzQzNC00Yjg5LThmNTEtMGUzYjJmOWI4Y2RlIiwidCI6ImY3ZmVmZWQ2LWYzNzktNDU3OS1iM2YwLWE0ZWZiZTFhN2RkZiJ9) |
| 2 | US Home Values | Real Estate | [View Report](https://app.powerbi.com/view?r=eyJrIjoiYTU4YzIyMzAtZDQ0MS00ZTY5LWI0M2UtY2ZiOWZlOTllNGU0IiwidCI6ImY3ZmVmZWQ2LWYzNzktNDU3OS1iM2YwLWE0ZWZiZTFhN2RkZiJ9) |


---

<!-- ============================================================
     PROJECT 1
     ============================================================ -->

## 📈 Project 1 — Economic Health Dashboard

**Category:** Macroeconomic Indicators  
**Data Source:** Federal Reserve Economic Data (FRED) API, St. Louis Fed  
**Tools Used:** Power BI Desktop · DAX · Power Query (M) · REST API · Power BI Service

### Overview

This report brings the key indicators of U.S. economic health into a single, always-current view: inflation, GDP growth, unemployment, consumer sentiment, the Fed funds rate, Treasury yields, and mortgage rates. It solves a common analyst problem: these indicators are published by different agencies on different schedules (daily, weekly, monthly, quarterly), which makes them hard to read side by side. The report pulls each series live from the FRED API, standardizes them into one model, and shows the latest reading with its change from the prior period. The primary audience could include strategy teams, finance and investment analysts, or executives who need a fast, plain-language read on where the economy stands and which direction it is moving.

### Key Features

- Scheduled daily refresh from eight FRED API series, combined in Power Query into a single unpivoted fact table with YoY, MoM, and annualized QoQ calculations.
- "Latest value" time intelligence that handles mixed reporting frequencies, so daily, monthly, and quarterly series each show their own most recent reading and prior-period comparison.
- Dynamic labels, arrows, and conditional colors that adapt to each metric (for example, rising inflation shows red while rising GDP shows green), plus dynamic number formats by indicator.
- A dynamically generated text summary on the Overview page that narrates current inflation, GDP, unemployment, and Fed rate readings.
- Disconnected date-range selector (last 5, 10, 20, or 30 years) driven by a DAX filter measure across every trend visual.
- Analytical measures such as Purchasing Power of $100 (CPI rebased to the selected range), Food & Energy CPI impact (headline minus core), and Mortgage Spread (30-year mortgage minus 10-year Treasury).
- Custom navigation built with action buttons across topic pages (Overview, Inflation, GDP, Rates, Relationships, Info), a custom theme, and a dedicated Info page for sources and definitions.

### Screenshot

<!-- TODO: Save a screenshot of the Overview page to /assets/images/project2.png -->
![Project 1 Dashboard Screenshot](assets/images/project1.png)

*Figure 1: Overview page showing the latest indicator readings with change vs. prior period, trend charts, and the dynamic economic health summary*

### 🔗 Interactive Report

<!-- TODO: Replace the iframe src and link below with your Publish to Web URL.
           Power BI Service → File → Embed Report → Publish to Web. -->

<iframe
  title="Economic Health Dashboard"
  width="100%"
  height="541.25"
  src="https://app.powerbi.com/view?r=eyJrIjoiZjUxMDAzOWUtYzQzNC00Yjg5LThmNTEtMGUzYjJmOWI4Y2RlIiwidCI6ImY3ZmVmZWQ2LWYzNzktNDU3OS1iM2YwLWE0ZWZiZTFhN2RkZiJ9"
  frameborder="0"
  allowFullScreen="true">
</iframe>

> 🔗 **[Open full interactive report in new tab](https://app.powerbi.com/view?r=eyJrIjoiZjUxMDAzOWUtYzQzNC00Yjg5LThmNTEtMGUzYjJmOWI4Y2RlIiwidCI6ImY3ZmVmZWQ2LWYzNzktNDU3OS1iM2YwLWE0ZWZiZTFhN2RkZiJ9)**

---

<!-- ============================================================
     PROJECT 2
     ============================================================ -->

## 🏡 Project 2 — US Home Values

**Category:** Real Estate Trends  
**Data Source:** Zillow Home Value Index (ZHVI) for All Homes Seasonally Adjusted  
**Tools Used:** Power BI Desktop · DAX · Power Query · Power BI Service

### Overview

This report provides a unified view of long‑term real estate trends across every U.S. state, with the ability to drill down into counties, cities, and even ZIP codes. It solves a core business problem by transforming fragmented housing data into clear insights on appreciation, volatility, and compound annual growth rates, helping leaders evaluate market performance and identify emerging opportunities. The primary audience of this report could include real estate analysts, investment teams, or strategy leaders who need fast, data‑driven visibility into how home values evolve over time and where growth is accelerating or slowing.

### Key Features

- Rules-based dynamic drillthrough button and field parameters to switch between county, city, and ZIP code detail.
- Collapsible filter pane and info panes utilizing bookmarks and bookmark navigation.
- Custom report page for tooltips with time-series data and CAGR calculation.
- Shape map visual with color gradient for growth rate by state.
- Time intelligence measures for calculating YoY growth rates.

### Screenshot

<!-- TODO: Replace the src with your actual screenshot path.
           Place images in an /assets/images/ folder in your repo. -->
![Project 2 Dashboard Screenshot](assets/images/project2.png)

*Figure 1: Homepage of the report showing collapsible filter pane, custom tooltip, and dynamic drillthrough button*

### 🔗 Interactive Report

<!-- TODO: Replace the iframe src with your Power BI Publish to Web embed URL.
           Get it from: Power BI Service → File → Embed Report → Publish to Web.
           Remove the HTML comment tags to activate the embed. -->

<iframe
  title="Us Home Values"
  width="100%"
  height="541.25"
  src="https://app.powerbi.com/view?r=eyJrIjoiYTU4YzIyMzAtZDQ0MS00ZTY5LWI0M2UtY2ZiOWZlOTllNGU0IiwidCI6ImY3ZmVmZWQ2LWYzNzktNDU3OS1iM2YwLWE0ZWZiZTFhN2RkZiJ9"
  frameborder="0"
  allowFullScreen="true">
</iframe>

> 🔗 **[Open full interactive report in new tab](https://app.powerbi.com/view?r=eyJrIjoiYTU4YzIyMzAtZDQ0MS00ZTY5LWI0M2UtY2ZiOWZlOTllNGU0IiwidCI6ImY3ZmVmZWQ2LWYzNzktNDU3OS1iM2YwLWE0ZWZiZTFhN2RkZiJ9)**

---

## 🎯 Target Roles

I'm exploring senior BI developer and analytics consulting opportunities focused on:

- Enterprise Power BI reporting strategy and governance
- Scalable self-service analytics platforms for business users
- Data-informed decision-making at the leadership level
- Analytics team mentorship and BI best-practice champions

**Open to:** BI Developer · Analytics Consultant · Senior BI Analyst · Analytics Engineering · BI Lead

---

## 📜 Certifications

| Certification | Issuer | Issued |
|---|---|---|
| Microsoft Certified: Azure Fundamentals (AZ-900) | Microsoft | August 2026 |

---
*Last updated: September 2026*
