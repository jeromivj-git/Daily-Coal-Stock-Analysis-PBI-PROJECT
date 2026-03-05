# 📊 Daily Coal Stock Monitoring and Consumption Analysis

## 📌 Project Overview
This project analyzes daily coal inventory data from thermal power stations across India to ensure efficient stock management and uninterrupted plant operations. Coal is a critical resource for power generation, and maintaining optimal stock levels is essential to prevent operational disruptions or excessive storage costs.

The dataset contains operational parameters such as daily coal receipt, daily consumption, actual stock levels, and normative stock levels. By comparing actual stock against normative requirements, the project evaluates whether coal inventory levels are within safe operational limits.

---

## 🎯 Project Objectives

### Monitor Coal Supply and Usage
- Track daily coal receipt and daily consumption
- Identify fluctuations in supply and demand

### Evaluate Stock Against Normative Levels
- Compare actual stock with predefined normative stock
- Measure deviation using Actual vs Normative %

### Identify Risk Conditions
- Detect potential coal shortages affecting operations
- Identify excess stock that increases storage costs

### Analyze Trends and Patterns
- Study daily and monthly consumption trends
- Understand stock movement over time

### Improve Inventory Planning
- Support forecasting of coal requirements
- Assist management in procurement planning

### Develop a Monitoring Dashboard
- Create interactive dashboards using Power BI

---

## 🗂️ Data Source

The dataset is obtained from the India Data Portal – Ministry of Power.

Dataset includes coal stock data from thermal power stations across India.

Domain: Energy  
Timeline: 2018 – 2025

Source Link:  
https://indiadataportal.com/p/power/r/mop-coal_stock-pl-dl-aaa

Key Data Fields:
- Mode of Transport
- Plant Capacity
- Normative Stock
- Actual Stock
- Daily Receipt
- Daily Consumption
- Plant Load Factor (PLF)
- Criticality Indicator
- Remarks

---

## 🛠️ Tools & Technologies

- Excel – Data cleaning, transformation, pivot tables
- Power BI – Data modelling, DAX calculations, dashboard visualization
- Power Query – Data preprocessing

---

## 🧹 Data Pre-Processing

### Data Cleaning
- Removed duplicate records
- Handled missing values
- Standardized column formats
- Created calculated fields

### Calculated Metrics

Daily Consumption

Daily_Consumption = Total Stock / Stock Days

Required Normative Stock

Req_Normative_Stock = Daily Requirement × Normative Stock Days

Actual vs Normative %

Actual_vs_Normative_% = (Total Stock / Req_Normative_Stock) × 100

---

## 🧩 Data Modeling

The dataset was structured into Fact and Dimension tables.

### Dimension Tables

Dim_Plant  
Plant ID | Plant Name | State | Sector | Utility | Capacity

Dim_Date  
Date ID | Date | Month | Year | Quarter

Dim_State  
State Code | State Name

### Fact Table

Fact_Stock  
Plant ID | Date ID | Mode of Transport | Daily Consumption | Daily Requirement | Indigenous Stock | Import Stock | Total Stock | Stock Days | PLF% | Critical | Remarks

### Relationships

Dim_State → Dim_Plant (1:M)  
Dim_Plant → Fact_Stock (1:M)  
Dim_Date → Fact_Stock (1:M)

---

## 📊 Exploratory Data Analysis

Analysis focused on:

- State-wise coal stock distribution
- Daily consumption vs requirement
- Indigenous vs import coal stock
- Transport mode distribution
- Power station capacity distribution
- Plant Load Factor (PLF) performance

---

## 📈 Key Visualizations

- Average PLF% across utilities
- Average PLF% across sectors
- Top 10 utilities by capacity
- State-wise capacity distribution
- Indigenous vs Import stock comparison
- Daily consumption vs daily requirement
- Distribution of power stations across states

---

## 💡 Key Insights

- Total daily requirement (13,074) exceeds actual consumption (11,695), indicating a national supply gap.
- 108 plants are classified as critical due to low coal stock levels.
- Average coal stock availability across plants is 8.23 days.
- Demand is heavily concentrated in Uttar Pradesh and Maharashtra.
- Bihar has the lowest operational stability with only 1.8 days of average coal stock.

---

## 🚨 Risk Analysis

High-Risk Regions
- West Bengal
- Chhattisgarh
- Bihar

Operational Risks
- Plants with less than 4 days of coal stock face shutdown risks.
- Supply chain disruptions may impact national power grid stability.

---

## 📊 Analytical Approach

Descriptive Analysis  
Summarizes current coal stock levels and operational metrics.

Diagnostic Analysis  
Identifies causes of supply shortages and consumption gaps.

Predictive Analysis  
Identifies future risks such as stock depletion and plant shutdowns.

Prescriptive Analysis  
Provides recommendations for improving coal logistics and supply management.

---

## 🚀 Recommendations

- Prioritize coal shipments to high-deficit states.
- Maintain minimum safety stock levels of at least 7 days.
- Improve rail-based coal transport logistics.
- Conduct operational efficiency audits for underperforming plants.
- Strengthen procurement planning and supply chain monitoring.

---

## 📌 Conclusion

- India faces a systemic coal supply gap between requirement and consumption.
- Over 100 power plants operate with critically low coal reserves.
- Significant regional disparities exist in coal distribution.
- Immediate logistics optimization is required to prevent power generation disruptions.

---



Project Type: Data Analysis / Power BI Dashboard  
Domain: Energy Analytics  
Purpose: Academic / Portfolio Project
