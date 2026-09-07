# Transportation Operations, SLA & Exception Analytics

An end-to-end transportation analytics project focused on monitoring shipment performance, SLA compliance, delivery exceptions, carrier performance, and route-level operational efficiency using **SQL, Microsoft Excel, and Power BI**.

## 📌 Project Overview

Transportation operations generate large volumes of shipment data that can be used to monitor service-level performance, identify delivery delays, and detect recurring operational issues.

This project analyzes **30,000 shipment records** to evaluate delivery performance across carriers and origin-destination routes. The analysis focuses on identifying SLA breaches, delay patterns, underperforming carriers/routes, and shipments that require operational attention.

The project follows a complete analytics workflow:

**Data Validation → Data Transformation → SQL Analysis → KPI Development → Exception Analysis → Power BI Dashboard → Operational Recommendations**

---

## 🎯 Objectives

- Monitor on-time delivery and SLA compliance.
- Identify delayed shipments and operational exceptions.
- Analyze carrier-level and route-level performance.
- Calculate key transportation performance indicators.
- Identify recurring delivery bottlenecks using historical data.
- Prioritize high-risk shipments using SLA-based escalation criteria.
- Develop actionable recommendations for improving operational efficiency.

---

## 🗂️ Dataset

**Dataset:** Supply Chain Shipments

**Records:** 30,000 shipment records

The dataset contains shipment-level information including order dates, dispatch dates, expected delivery dates, actual delivery dates, carriers, routes, shipment weight, freight cost, and delivery performance indicators.

> **Note:** The dataset is used for educational and portfolio purposes. It does not represent Amazon's internal transportation data.

---

## 🛠️ Tools & Technologies

### SQL
- Data querying
- JOINs
- GROUP BY
- Aggregate functions
- CASE statements
- Subqueries
- KPI calculations
- Carrier and route performance analysis
- Exception analysis

### Microsoft Excel
- Data cleaning and validation
- Calculated fields
- PivotTables
- KPI analysis
- Delay categorization
- Performance analysis

### Power BI
- Data modeling
- DAX measures
- KPI cards
- Interactive dashboards
- Trend analysis
- Carrier performance monitoring
- Route performance analysis
- Exception monitoring

---

## 📊 Key KPIs

The project tracks transportation-focused KPIs such as:

- Total Shipments
- On-Time Delivery %
- SLA Compliance %
- SLA Breach %
- Average Delivery Delay
- Delayed Shipment Count
- Exception Rate
- Carrier Performance
- Route Performance
- High-Risk Shipment Count
- Shipment Volume Trends

---

## 🚦 SLA & Exception Framework

For this portfolio project, the **expected delivery date is treated as the service-level target**.

### SLA Breach

A shipment is classified as an SLA breach when:

`Actual Delivery Date > Expected Delivery Date`

### Delay Classification

Shipments are categorized based on delivery delay to make operational performance easier to monitor.

Example categories:

- On Time
- 1–2 Days Delayed
- 3–5 Days Delayed
- More Than 5 Days Delayed

### Escalation Risk

A project-defined escalation rule is used to identify shipments with significant SLA breaches that may require prioritization.

> These escalation criteria are analytical assumptions created for this project and are not Amazon operational policies.

---

## 📈 Power BI Dashboard

The Power BI dashboard is designed as an operational monitoring tool with multiple analytical views.

### Operations Overview
Provides a high-level view of:

- Total shipments
- On-time delivery
- SLA compliance
- Average delay
- Exception volume
- Shipment trends

### Exception Monitoring
Focuses on:

- Delayed shipments
- SLA breaches
- High-risk shipments
- Delay categories
- Historical exception trends

### Carrier & Route Performance
Analyzes:

- Carrier-wise SLA performance
- Carrier-wise delay rates
- Route-level performance
- High-performing and underperforming routes
- Shipment volume by carrier and route

---

## 🔎 Analytical Approach

The analysis follows these stages:

1. **Data Validation**
   - Checked missing values and inconsistent records.
   - Validated date fields and shipment-level information.

2. **Data Transformation**
   - Created calculated operational fields.
   - Calculated delivery delay.
   - Classified SLA breaches and delay categories.
   - Created escalation-risk indicators.

3. **SQL Analysis**
   - Analyzed shipment performance.
   - Compared carriers and routes.
   - Identified recurring delay patterns.
   - Calculated operational KPIs.

4. **Excel Analysis**
   - Performed validation and exploratory analysis.
   - Created PivotTables and supporting calculations.
   - Reviewed shipment and carrier performance.

5. **Power BI Visualization**
   - Developed an interactive operational dashboard.
   - Created KPI measures and performance views.
   - Added exception monitoring and filtering capabilities.

6. **Operational Insights**
   - Identified performance bottlenecks.
   - Highlighted recurring carrier and route issues.
   - Developed recommendations based on historical performance.

---

## 💡 Business Questions

The project answers questions such as:

- What percentage of shipments are delivered on time?
- Which carriers have the highest SLA breach rates?
- Which routes experience the most delivery delays?
- How does delivery performance change over time?
- Where are the largest operational bottlenecks?
- Which shipments require prioritization based on escalation criteria?
- Which carriers or routes should be investigated for process improvement?

---

## 📁 Repository Structure

```text
Transportation-Operations-SLA-Analytics/
│
├── README.md
│
├── data/
│   └── supply_chain_shipments.csv
│
├── sql/
│   └── transportation_analysis.sql
│
├── excel/
│   └── transportation_analysis.xlsx
│
├── powerbi/
│   └── transportation_operations_dashboard.pbix
│
└── images/
    ├── dashboard_overview.png
    └── dashboard_exceptions.png
