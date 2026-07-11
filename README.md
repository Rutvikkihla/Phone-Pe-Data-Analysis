# PhonePe Transaction Analytics

---

## 📌 Overview
A complete **end-to-end data analytics project** built on a 100K PhonePe transaction dataset covering the full year 2024. The project follows a real-world analyst workflow - raw data loaded in Excel, visualized in a multi-page Power BI dashboard.
The objective is to uncover patterns in payment behavior, service usage, failure reasons, and monthly trends across four business verticals: **Money Transfer, Recharge & Bills, Loans, and Insurance**.

---

 
## 📂 Dataset
 
| Property | Details |
|---|---|
| **File** | `Phonepe-1Lakh-Dataset.xlsx` |
| **Total Records** | 1,00,000 transactions |
| **Period** | 01 Jan 2024 – 30 Dec 2024 |
| **Users** | 1,00,000 unique users · Age range: 18–60 · Avg age: 39 |
 
### Sheets Breakdown
 
| Sheet | Rows | Key Columns |
|---|---|---|
| `All_Users` | 1,00,000 | User_ID, Name, Age, Join_Date |
| `All_Transactions` | 1,00,000 | Transaction_ID, Amount, User_ID, Service, Service Type, Payment_Status, Reason, Date |
| `Recharge_Bills` | 50,000 | Transaction_ID, User_ID, Recharge_Type, Amount, Date, Payment_Status, Reason |
| `Money_Transfer` | 1,00,000 | Transaction_ID, User_ID, Transfer_Type, Amount, Date, Payment_Status, Reason |
| `Loans` | 50,000 | Transaction_ID, User_ID, Loan_Type, Loan_Amount, Date, Payment_Status, Reason |
| `Insurance` | 50,000 | Transaction_ID, User_ID, Insurance_Type, Premium, Date, Payment_Status, Reason |
 
---

## 🛠️ Tools & Technologies

| Layer | Tool |

| **Dashboard** | Microsoft Power BI |
| **Version Control** | Git & GitHub |

---

## 🔄 Project Steps


### Step 1 — 📊 Power BI Dashboard
 
- Connected Power BI to MySQL using the native MySQL connector
- Built **5 interactive dashboard pages** with a consistent PhonePe purple theme:
- 
| Page | Key Visuals |
|---|---|
| **Overview** | KPI cards (total transactions, amount, success/failure count), monthly trend line, service bar chart, failure pie chart |
| **Loans** | Loan amount by type (bar), monthly disbursement (line), payment status (donut) |
| **Insurance** | Premium by insurance type (bar), monthly trend (line), failure reasons (pie) |
| **Money Transfer & Recharge** | Transfer channel breakdown, recharge types, monthly amount line |
 
- Added a **date range slicer** (1 Jan – 30 Dec 2024) that filters all visuals simultaneously
- Applied drill-through on Service Type for transaction-level detail
---
 
### Step 1 — 📝 Report
 
- Written in structured format: Objective → Methodology → Key Findings → Recommendations
- Charts and tables sourced from Power BI and Python notebooks
- Exported as PDF for sharing and submission
---

## 📊 Dashboard Preview
 
> 4-page interactive Power BI dashboard with date slicer, drill-throughs, and PhonePe purple branding.
 
| Page Preview|
|---|
| Home |
|![PhonePe Dashboard](PhonePe%20Dashboard_page-0001.jpg)
| Overview | 
![PhonePe Dashboard](PhonePe%20Dashboard_page-0002.jpg)
| Loans | 
![PhonePe Dashboard](PhonePe%20Dashboard_page-0003.jpg)
| Insurance | 
![PhonePe Dashboard](PhonePe%20Dashboard_page-0004.jpg)
| Money Transfer & Recharge | 
![PhonePe Dashboard](PhonePe%20Dashboard_page-0005.jpg)
  
---

## 📈 Key Results & Insights
 
| | Insight |
|---|---|
| ✅ | **96.16% overall success rate** across 1,00,000 transactions |
| ❌ | Top 3 failure reasons: **Server Error (34%)**, **Wrong PIN (33%)**, **Insufficient Amount (32%)** |
| 💸 | **Total transaction value: ₹17.65 Crore** · Average transaction: ₹1,765 |
| 🏦 | **Auto Loan leads** at ₹64.36 Cr, followed by Mutual Fund (₹63.42 Cr) and Gold Loan (₹63.24 Cr) |
| 🛡️ | **Car Insurance** tops the segment at ₹12.93 Cr — all four types are closely distributed |
| 📲 | **UPI ID is the most-used transfer channel** (₹63.16M); To Self Account is a close second |
| 🔌 | **Electricity Bill** leads Recharge & Bills (₹12.82M), followed by DTH and Mobile Recharge |
| 📅 | **July and March** are peak months for transaction volumes across multiple categories |
| 👥 | User base spans **age 18–60** with an average age of **39 years** |

---


## 📄 License

This project is for educational and portfolio purposes. Dataset used is synthetic/anonymized.
