📊 Daily Coal Stock Monitoring and Consumption Analysis
🟤 Project Overview

This project focuses on analyzing daily coal inventory data to ensure efficient stock management and uninterrupted plant operations. Coal is a critical resource for energy generation, and maintaining optimal stock levels is essential to avoid operational risks and high storage costs.

The dataset includes key operational parameters such as:

Daily coal receipt

Daily coal consumption

Actual stock levels

Normative stock requirements

By comparing actual stock vs normative stock, this project evaluates inventory performance and identifies risk conditions.

🎯 Project Objectives

Monitor coal supply and consumption patterns.

Evaluate stock levels against normative benchmarks.

Detect critical shortage and excess stock conditions.

Analyze trends in coal inventory movement.

Support procurement and logistics decision-making.

Build interactive Power BI dashboards.

🗂️ Data Source

The dataset is obtained from the India Data Portal – Ministry of Power.

Domain: Energy Sector

Data Coverage: Thermal power stations across India

Time Period: 2018 – 2025

Data Fields Include:

Mode of transport

Plant capacity

Normative stock levels

Coal receipts and consumption

Plant load factor (PLF)

Critical condition indicators

🔗 Source Link:
https://indiadataportal.com/p/power/r/mop-coal_stock-pl-dl-aaa

🛠️ Tools & Technologies

Microsoft Excel – Data Cleaning, Transformation, Pivot Tables

Power BI – Data Modeling, DAX Calculations, Visualization

Power Query – Data preprocessing and transformation

GitHub / Documentation Tools – Project hosting and reporting

🧹 Data Pre-Processing
Data Cleaning & Transformation

Removed duplicate records.

Handled missing values.

Standardized formats for date and numeric fields.

Created calculated metrics.

Calculated Metrics

Daily Consumption

Daily Consumption = Total Stock / Stock Days

Required Normative Stock

Required Normative Stock = Daily Requirement × Normative Days

Actual vs Normative Stock Percentage

( Total Stock / Required Normative Stock ) × 100
Data Modeling Structure
Dimension Tables

Dim_Plant

Dim_Date

Dim_State

Fact Table

Fact_Stock

Relationships

Dim_State → Dim_Plant (1 : Many)

Dim_Plant → Fact_Stock (1 : Many)

Dim_Date → Fact_Stock (1 : Many)

📊 Exploratory Data Analysis (EDA)

Analysis focused on:

State-wise coal stock distribution

Daily consumption vs requirement comparison

Plant load factor performance

Transport mode distribution

Power station capacity distribution

💡 Key Insights

Total daily requirement exceeds actual consumption nationally, indicating a supply deficit.

Approximately 108 plants are marked as critical due to low stock levels.

Average coal stock is sufficient for about 8 days of operations.

Demand is highly concentrated in major states such as Uttar Pradesh and Maharashtra.

Bihar shows very low operational safety margins with less than 40% demand fulfillment.

🚨 Risk Analysis
High Risk States

West Bengal

Chhattisgarh

Bihar

Operational Risks Identified

Plants with less than 4 days stock are at shutdown risk.

Supply chain constraints impact power generation efficiency.

📈 Analysis Types Performed
Descriptive Analysis

Total national consumption vs requirement.

Stock availability statistics.

Diagnostic Analysis

Supply-side shortages.

Correlation between stock and consumption.

Predictive Analysis

Future depletion risks.

Power outage probability assessment.

Prescriptive Analysis

Supply chain optimization recommendations.

🚀 Recommendations

Prioritize coal supply to high deficit states.

Maintain minimum safety stock levels (7+ days).

Improve rail-based coal transport logistics.

Conduct efficiency audits for underperforming plants.

Optimize procurement and storage strategies.

⚙️ How to Use

Download the Power BI .pbix file.

Open using Power BI Desktop.

Use filters and slicers to explore:

State-wise performance

Plant-level metrics

Monthly trends

Critical plant analysis

📌 Conclusion

India faces a persistent coal supply gap between demand and consumption.

Energy distribution is uneven across states.

Immediate logistical and policy actions are required to maintain grid stability.

