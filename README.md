# 🚗⚡ Modeling India's ICE-to-EV Transition

**Adoption Trends, Infrastructure Impact & Forecasts**

---

## 📌 Project Overview

India's automotive sector is undergoing a gradual transition from Internal Combustion Engine (ICE) vehicles to Electric Vehicles (EVs). While EV adoption is increasing due to policy incentives, environmental concerns, and technological advancements, the transition remains uneven across states and vehicle segments.

This project presents an **interactive Power BI dashboard** designed to:

- Analyze EV adoption patterns across Indian states and vehicle categories
- Examine the role of charging infrastructure in influencing EV adoption
- Explain why adoption differs regionally
- Forecast future EV adoption trends over the next 2–3 years

The dashboard is built as part of a case study competition, focusing on **interpretability, data-driven insights**, and decision support for policymakers and industry stakeholders.

---

## 🎯 Objectives

The primary objectives of this project are to:

- Analyze state-wise and segment-wise EV adoption
- Track EV adoption trends over time
- Understand the relationship between charging infrastructure and EV sales
- Identify regional disparities in EV adoption
- Forecast future EV adoption growth for India
- Provide interpretable insights rather than black-box predictions

---

## 📊 Dashboard Features

The Power BI dashboard includes the following analytical components:

### 1️⃣ EV Adoption Overview
- Total EV sales across India
- EV adoption by state
- EV adoption by vehicle category (2W, 3W, 4W, etc.)
- Interactive year-based filtering

### 2️⃣ Adoption Trends Over Time
- Year-wise EV adoption growth
- Segment-wise EV adoption trends
- Identification of acceleration periods in EV adoption

### 3️⃣ Infrastructure Impact Analysis
- Comparison of charging infrastructure growth vs EV adoption
- Infrastructure efficiency metric (EVs per charging station)
- Identification of states with:
  - Infrastructure surplus
  - Infrastructure deficit
  - Balanced readiness

### 4️⃣ Predictive Analysis (Forecasting)
- Time-series forecasting of EV adoption for the next 2–3 years
- Confidence intervals to represent uncertainty
- Trend-based, explainable forecasting using historical data

---

## 🗂️ Datasets Used

### 1️⃣ Organizer-Provided Dataset (Primary)

**EV Charging Infrastructure Dataset**

| Column | Description |
|--------|-------------|
| State | Indian state/UT |
| Year | Reporting year |
| Number of charging stations | Count of operational charging stations |
| Percentage of fast chargers | % of fast charging infrastructure |
| Urban coverage percentage | % coverage in urban areas |

*This dataset represents the infrastructure readiness side of the EV ecosystem.*

### 2️⃣ External Dataset (Supplementary)

**Electric Vehicle Sales by State**

| Column | Description |
|--------|-------------|
| State | Indian state/UT |
| Date / Year | Time period |
| Vehicle category | 2W, 3W, 4W classification |
| EV sales quantity | Number of units sold |

*This dataset represents actual EV adoption and demand.*

> ⚠️ **Note:** Only one external dataset was intentionally used to comply with case competition constraints and to maintain analytical clarity.

---

## 🧹 Data Cleaning & Preparation

All data preparation was done manually using **Power BI Power Query**, without automated ML pipelines.

### Key Cleaning Steps:

1. Removed duplicate and irrelevant columns
2. Filtered out zero-sales records
3. Aggregated daily-level EV sales data to State–Year–Vehicle Category level
4. Standardized column naming conventions across datasets
5. Created a composite State–Year key to ensure correct table relationships
6. Verified data types (text, numeric, date) for accurate modeling

**These steps ensured:**
- Reduced noise
- Correct aggregation
- Accurate relationships
- Reliable visual outputs

---

## 🔗 Data Modeling Approach

- **EV sales data** used as the fact table
- **Charging infrastructure data** used as an explanatory table
- Tables connected using a **State–Year composite key**
- Avoided many-to-many relationships to maintain model integrity
- All calculations implemented using **DAX measures**

This modeling approach ensures trustworthy analytics and avoids silent aggregation errors.

---

## 🔮 Prediction Methodology

### Forecasting Technique Used:
**Power BI Time-Series Forecasting (Exponential Smoothing)**

### Why This Approach:
- Transparent and interpretable
- Suitable for short-term forecasting (2–3 years)
- Accepted in business and policy analysis
- Avoids black-box machine learning models

### Prediction Output:
- Forecasted EV adoption trend for India
- Confidence interval bands to reflect uncertainty
- Insight into the direction and pace of the ICE-to-EV transition

> 📝 The forecasts are trend-based, not causal claims, and are presented as decision-support signals.

---

## 🧠 Key Insights

- ✅ EV adoption in India is highly uneven across states
- ✅ Two-wheelers and three-wheelers dominate EV adoption
- ✅ Charging infrastructure growth is largely policy-led and urban-focused
- ✅ Some states show infrastructure-first strategies, while others show demand-led adoption
- ✅ Forecasts indicate continued growth in EV adoption, with widening gaps between early and late adopters

---

## 🛠️ Tools & Technologies

- **Power BI Desktop** - Dashboard development
- **Power Query** - Data cleaning & transformation
- **DAX** - Measures & metrics
- **Excel / CSV** - Data sources

---

## 📁 Repository Structure

```
📦 EV-Transition-India
 ┣ 📂 data
 ┃ ┣ 📄 ev_charging_infrastructure.csv
 ┃ ┗ 📄 ev.csv
 ┣ 📂 dashboard
 ┃ ┗ 📄 EV_Transition_India_Led_Zeppelin.pbix
 ┗ 📄 README.md
```

---

## 🏁 Conclusion

This project demonstrates how data-driven dashboards, combined with interpretable analytics and forecasting, can be used to understand and explain the ICE-to-EV transition in India. The framework is designed to support:

- 📊 Policy planning
- 🔌 Infrastructure investment decisions
- 📈 Market analysis

All while remaining **transparent** and **competition-appropriate**.

---

## 📧 Contact & Contributions

For questions, suggestions, or collaboration opportunities, please feel free to reach out or open an issue.

---

**Made with ⚡ for sustainable mobility in India**
