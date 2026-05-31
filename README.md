# 🏦 Banking Risk & Analytics Dashboard

> An end-to-end banking analytics project built with **Power BI**, **Python**, and **MySQL** — designed to analyze client risk, deposit behavior, and loan exposure across a 3,000-client dataset.

---

## 📌 Overview

This project simulates a real-world banking analytics workflow. Raw client and financial data is explored in Python, stored in a local MySQL database, and visualized through a multi-page Power BI dashboard. The primary goal is **risk analysis** — identifying which client segments carry the highest financial exposure and how deposit vs. lending behavior varies across demographics.

---

## 🛠️ Tech Stack

| Layer | Tool |
|---|---|
| Exploratory Analysis | Python (Pandas, Matplotlib, Seaborn) |
| Data Storage | MySQL + MySQL Workbench |
| Dashboard & Reporting | Microsoft Power BI Desktop |

---

## 📊 Dashboard Pages

### 🏠 Home
Landing page with top-level KPIs and navigation to other sections.

| Metric | Value |
|---|---|
| Total Clients | 3,000 |
| Total Loans | 4.38bn |
| Total Deposits | 3.77bn |
| Checking Accounts | 963.28M |
| Saving Accounts | 698.73M |
| Business Lending | 2.60bn |

Filters: Joining Year, Gender

---

### 📈 Loan Analysis
Breaks down the lending portfolio by client risk weighting, occupation, banking relationship type, and demographics. Helps identify over-exposed segments.

### 💰 Deposit Analysis
Explores deposit composition across:
- **Banking Relationship** — Commercial, Institutional, Private Bank, Retail
- **Income Band** — Low / Mid / High
- **Occupation & Nationality** — bar chart breakdowns
- **Gender & Institutional Advisor** — slicer-driven filtering

Key metrics: Total Deposit, Bank Deposit, Saving Account Amount, Checking AA

### 📋 Summary
Consolidated executive view aggregating risk, deposit health, and loan performance in one page.

---

## 🗂️ Dataset Columns

`Client ID` · `Name` · `Age` · `Location ID` · `Joined Bank` · `Banking Contact` · `Nationality` · `Occupation` · `Fee Structure` · `Loyalty Classification` · `Estimated Income` · `Superannuation Savings` · `Amount of Credit Cards` · `Credit Card Balance` · `Bank Loans` · `Bank Deposits` · `Checking Accounts` · `Saving Accounts` · `Foreign Currency Account` · `Business Lending` · `Properties Owned` · `Risk Weighting` · `BRId` · `GenderId` · `IAId`

---

## 🔍 Python EDA Highlights

Before loading into Power BI, the dataset was explored in Python:

- Null detection and handling strategy
- Distribution analysis of `Risk Weighting`, `Estimated Income`, and `Bank Loans`
- Outlier identification in credit card and business lending columns
- Correlation analysis between key financial variables
- Client segmentation by loyalty classification and occupation

---

## 🗄️ MySQL Setup

Data is stored in a local MySQL server and queried directly by Power BI. MySQL Workbench was used for schema design, data inspection, and query testing.

---


Then open `Banking_Dashboard.pbix` in Power BI Desktop, go to **Transform Data → Data Source Settings**, update the MySQL connection string, and hit Refresh.

---


## 👤 Author

**Abdul Wahab** — Data Analyst | Power BI Developer  
 https://github.com/Wahab-300/

> Dataset is fictional and used for portfolio/educational purposes only.
