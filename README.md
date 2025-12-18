# 📊 Loan Portfolio Risk & Performance Analytics Dashboard

## 🔍 Project Overview
This project delivers an **end-to-end loan portfolio analytics solution** using **MS SQL Server and Power BI** to analyze **38,000+ loan records** and monitor **$435M+ in funded loans**.  
The goal is to help stakeholders **assess portfolio health, identify credit risk concentration, and support data-driven lending decisions** through interactive dashboards and analytical insights.

Unlike basic reporting dashboards, this project focuses on **risk segmentation, recovery analysis, and actionable recommendations** for loan approval and portfolio optimization.

---

## 🧠 Business Problem
Financial institutions must balance **loan growth** with **credit risk control**.  
This project addresses key decision-making questions such as:

- Which borrower segments contribute disproportionately to bad loans?
- Are higher interest rates adequately compensating for default risk?
- How do borrower attributes (DTI, loan grade, employment length, home ownership) affect repayment?
- Where is risk concentrated across loan purposes and geographies?

The objective is to move beyond descriptive reporting and provide **decision-support analytics**.

---

## 📂 Dataset Description
- **Records:** 38,000+ loan applications  
- **Key attributes:**
  - Loan grade & sub-grade  
  - Interest rate  
  - Debt-to-Income (DTI) ratio  
  - Employment length  
  - Loan purpose  
  - Home ownership  
  - State (geography)  
  - Funded amount & amount received  
  - Loan status (Fully Paid, Current, Charged Off)

---

## ⚙️ Analytical Approach

### 1️⃣ Data Preparation (MS SQL Server)
- Cleaned and transformed raw loan data
- Used **CTEs, window functions, date logic, and aggregations**
- Built analysis-ready tables for BI consumption

### 2️⃣ Data Modeling & Measures (Power BI)
- Optimized data model and relationships
- Created **DAX measures** for:
  - MTD & MoM KPIs
  - Funded vs received amount
  - Average interest rate & DTI
  - Good vs bad loan segmentation

### 3️⃣ Portfolio Segmentation
Analysis performed across:
- Loan grade
- Loan purpose
- DTI buckets
- Employment length
- Home ownership
- Geography (state-level)

### 4️⃣ Risk vs Recovery Analysis
- Compared funded vs received amounts
- Evaluated contribution of bad loans to portfolio losses
- Identified risk concentration drivers

---

## 📊 Dashboard Structure

### 🔹 Summary Dashboard
- High-level KPIs:
  - Total loan applications (MTD & MoM)
  - Total funded amount
  - Total amount received
  - Average interest rate
  - Average DTI
- **Good vs Bad Loan distribution** for portfolio health assessment

### 🔹 Overview Dashboard
- Monthly loan funding and recovery trends
- State-wise performance analysis
- Purpose-wise contribution
- Home ownership impact on repayment

### 🔹 Details Dashboard
- Record-level drill-down
- Interactive filters by:
  - State
  - Loan grade
  - Purpose
  - Loan status

---

## 🔍 Key Insights
- **~86% of loans are good loans**, while the remaining **~14% contribute disproportionately to funded losses**, indicating risk concentration.
- Lower loan grades (C–E) show **higher default risk**, and higher interest rates do **not fully compensate** for losses.
- **Debt consolidation loans dominate portfolio volume** and significantly amplify bad-loan exposure.
- Borrowers with **10+ years of employment** demonstrate stronger repayment reliability.
- **Renters exhibit higher DTI and default risk** compared to mortgage holders.
- Certain states consistently show **higher charge-off rates**, highlighting regional risk patterns.

---

## 📌 Business Recommendations
- Apply **risk-adjusted approval criteria** for high-DTI and low-grade borrowers.
- Re-price or cap loan amounts for high-risk segments instead of blanket rejection.
- Reduce concentration in **debt consolidation loans** through portfolio diversification.
- Introduce **region-specific underwriting controls** for high-risk states.
- Track early-warning KPIs such as rising DTI and declining recovery ratios.

---

## 💼 Business Impact
This solution enables:
- Faster and more accurate **credit risk assessment**
- Identification of high-risk borrower segments
- Data-backed policy adjustments for loan approvals
- Reduced manual reporting via SQL-to-Power BI automation
- Improved portfolio stability and recovery outcomes

---

## 🛠️ Tech Stack
- **Power BI** – Data modeling, DAX, KPIs, interactive dashboards  
- **MS SQL Server** – Data transformation, CTEs, window functions  
- **DAX** – Time intelligence and advanced measures  
- **Power Query** – Data cleaning and processing  

---

## Repository Structure
```text
financial_loan/
├── Dataset/
├── Loan_SQLQuery/
│   └── SQL queries and transformations
├── Bank Loan Analysis/
│   ├── Power BI (.pbix) file
│   ├── Screenshots/
│   │   └── Dashboard images
├── README.md
│   └── Project documentation
```

---

## 📈 Output Preview
The dashboards provide:
- Loan application trends by time, geography, and borrower profile  
- Funded vs received amount comparisons  
- Good vs bad loan risk segmentation  
- Interactive drill-down for detailed analysis  

---

