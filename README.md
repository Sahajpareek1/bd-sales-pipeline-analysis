# BD Sales Pipeline Analysis & Dashboard

## 📌 Project Overview
This project focuses on **cleaning, analyzing, and visualizing** a Business Development (BD) sales pipeline dataset.  
The dataset contains **900+ opportunities** spanning multiple stages of the sales process, with details such as client information, lead source, deal size, and revenue.

The final output is an **interactive Power BI dashboard** that provides insights into the sales pipeline performance, win rates, deal values, and conversion trends.

---

## 🗂 Dataset Overview
**Source:** Provided as part of an assessment task  
**Rows:** ~900  
**Columns:** Opportunity details, BD representatives, client info, deal sizes, dates, and pipeline stages.

Key columns:
- `Opportunity_ID`
- `BD_Team` / `BD_Representative`
- `Client_Name` / `Industry` / `Region`
- `Lead_Source` / `Campaign` / `Lead_Score`
- `Current_Stage`
- `Initial_Contact_Date` / `Deal_Closed_Date`
- `Expected_Deal_Size` / `Actual_Revenue`

---

## 🧹 Data Cleaning & Preparation
**Steps performed in Python (Pandas):**
- **Handled missing values:**
  - `BD_Representative` → Filled with `"Unknown"`
  - `Lead_Source` → Filled with `"Unknown"`
  - `Lead_Score` → Filled with median
  - `Expected_Deal_Size` → Filled with median
  - `Industry` & `Campaign` → Pending decision → `"Unknown"`
  - `Deal_Closed_Date` → Left as missing (mostly ongoing deals)
- **Corrected data types:**
  - Converted date columns to `datetime`
  - Converted numeric columns to appropriate types
- **Standardized formatting:**
  - Fixed inconsistent capitalization and spelling in `Region`, `Client_Name`, and `BD_Representative`
- **Removed duplicates**
- **No significant outliers detected**

A detailed cleaning report is available in `data_cleaning_report.md`.

---

## 📊 Power BI Dashboard
**Main features:**
- **KPI Cards:**
  - Total Opportunities
  - Total Expected Deal Size
  - Total Actual Revenue
  - Win Rate %
  - Average Deal Size
  - Average Lead Score
  - Pipeline Value
- **Visuals:**
  - Funnel chart: Sales Pipeline by Stage
  - Bar charts: Revenue by Region & BD Representative
  - Line chart: Revenue trend by month
  - Pie chart: Lead Source share
  - Table: Detailed opportunity list with filters
- **Slicers:**
  - Region
  - Industry
  - Lead Source
  - Date

---

## 📈 Key Insights
- **Most drop-off** occurs at the `Proposal Sent` stage.
- **APAC region** shows higher win rates despite fewer opportunities.
- **Referral leads** yield higher deal values compared to other lead sources.
- Large share of deals are still in early pipeline stages, indicating future potential revenue.

---

## 🚀 Recommended Actions
- Focus BD efforts on **improving proposal-to-close conversion**.
- Increase investment in **high-performing lead sources** like referrals.
- Strengthen engagement with large deals in APAC to accelerate closure.

---

---

## 🛠 Tools Used
- **Python** (Pandas, NumPy) – Data cleaning & preparation
- **Power BI** – Dashboard creation & analysis
- **Excel** – Initial dataset inspection

---

## 📬 Contact
For questions or collaboration:
**Your Name** – prksahaj@gmail.com

