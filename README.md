# 📊 Sales Analytics Dashboard — Excel & Power Pivot
 
<div align="center">
<img src="https://img.shields.io/badge/Microsoft%20Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white" alt="Excel"/>
<img src="https://img.shields.io/badge/Power%20Pivot-0078D4?style=for-the-badge&logo=microsoft&logoColor=white" alt="Power Pivot"/>
<img src="https://img.shields.io/badge/Power%20Query-0EA5E9?style=for-the-badge&logo=microsoft&logoColor=white" alt="Power Query"/>
<img src="https://img.shields.io/badge/Schema-Star%20Schema-22C55E?style=for-the-badge" alt="Star Schema"/>
<img src="https://img.shields.io/badge/Records-9%2C994%20Rows-6366F1?style=for-the-badge" alt="Records"/>
<img src="https://img.shields.io/badge/Status-Completed-16a34a?style=for-the-badge" alt="Status"/>
<br/><br/>
 
<strong>A fully interactive Excel dashboard powered by Power Pivot and Power Query — analyzing 9,994 transactions across customers, products, cities, and shipping modes to surface actionable sales, profit, and quantity insights.</strong>
 
</div>
---
 
## 🗂️ Table of Contents
 
- [Project Overview](#-project-overview)
- [Project Workflow](#-project-workflow)
- [Dashboard Highlights](#-dashboard-highlights)
- [Pivot Tables Analysis](#-pivot-tables-analysis)
- [Data Model](#-data-model)
- [Key KPIs at a Glance](#-key-kpis-at-a-glance)
- [Tools & Technologies](#-tools--technologies)
- [Project Structure](#-project-structure)
- [How to Use](#-how-to-use)
---
 
## 🎯 Project Overview
 
This project analyzes **retail sales data** across the United States to help management understand:
 
- 👥 **Which customers** generate the highest sales and quantities
- 🏙️ **Which cities** are top and bottom performers
- 📦 **Which products and categories** drive the most revenue
- 📅 **Monthly and quarterly trends** in sales and profit
- 🚚 **Which shipping modes** are most used
| Feature | Details |
|---|---|
| 📁 Excel File | `Excel_Data_Analysis_Project.xlsx` |
| 📄 Sheets | Pivot Tables · Dashboard |
| 🗃️ Data Model | Star Schema (Power Pivot) |
| 🔄 ETL | Power Query (5 queries cleaned) |
| 📊 Total Records | 9,994 transactions |
| 🏷️ Categories | 3 (Furniture · Office Supplies · Technology) |
| 🏷️ Sub-Categories | 17 sub-categories |
| 🚚 Ship Modes | 4 (Standard · Second · First · Same Day) |
 
---
 
## 🔄 Project Workflow
 
```
Raw Data (CSV / Excel)
        │
        ▼
┌───────────────────────────────┐
│  🔄 Power Query (ETL)         │
│  • Filtered null rows         │
│  • Replaced incorrect values  │
│  • Renamed & removed columns  │
│  • Fixed data types           │
│  • Split & expanded columns   │
│  • 5 cleaned queries loaded   │
└──────────────┬────────────────┘
               │
               ▼
┌───────────────────────────────┐
│  🗃️ Power Pivot (Data Model)  │
│  • Built Star Schema          │
│  • Defined relationships      │
│  • Created DAX measures       │
└──────────────┬────────────────┘
               │
               ▼
┌───────────────────────────────┐
│  📋 Pivot Tables Sheet        │
│  • 10+ analysis pivot tables  │
│  • Top/Bottom rankings        │
│  • Monthly & quarterly trends │
└──────────────┬────────────────┘
               │
               ▼
┌───────────────────────────────┐
│  📊 Dashboard Sheet           │
│  • Interactive slicers        │
│  • 8+ dynamic charts          │
│  • KPI summary cards          │
└───────────────────────────────┘
```
 
---
 
## 📊 Dashboard Highlights
 
The **Dashboard** sheet is the main interactive view — it updates dynamically based on 3 slicers.
 
**Slicers:**
- 📅 **Quarter** — Filter by Q1, Q2, Q3, Q4
- 🏷️ **Category** — Furniture · Office Supplies · Technology
- 🏷️ **Sub-Category** — All 17 sub-categories
**KPI Cards (top of dashboard):**
 
| KPI | Value |
|---|---|
| 💰 Total Sales (T-Sales) | **$2,297,201** |
| 📦 Total Quantity (T-Quantity) | **37,873 units** |
| 💵 Total Profit (T-Profit) | **$286,397** |
| 🏷️ Total Discount (T-Discount) | **$1,561** |
 
**Charts in Dashboard:**
 
| Chart | Type | Insight |
|---|---|---|
| Top 10 Customers by Sales & Quantity | Combo (Bar + Line) | Sean Miller is #1 with $25,043 |
| Top 10 Cities by Sales & Quantity | Combo (Bar + Line) | Los Angeles leads at $141,770 |
| T-Sales by Month | Line Chart | Strong upward trend Nov–Dec |
| T-Profit by Month | Line Chart | Profit peaks in Q4 |
| Top Products by Sales | Bar Chart | Canon imageCLASS 2200 leads |
| Sub-Category by Sales & Quantity | Combo Chart | Full breakdown across all 17 |
| T-Sales by Ship Mode | Donut Chart | Standard Class dominates |
 
---
 
## 📋 Pivot Tables Analysis
 
The **Pivot Tables** sheet contains all the detailed analysis tables:
 
### 💰 Sales & Profit by Month
 
| Month | T-Sales | T-Profit |
|---|---|---|
| Jan | $94,924 | $9,134 |
| Mar | $205,005 | $28,594 |
| Sep | $307,649 | $36,857 |
| Nov | $352,461 | $35,468 |
| Dec | $325,293 | $43,369 |
| **Total** | **$2,297,201** | **$286,397** |
 
### 🏙️ Top 10 Cities by Sales
 
| City | T-Sales | T-Quantity |
|---|---|---|
| 🥇 Los Angeles | $141,770 | 2,766 |
| 🥈 New York City | $210,926 | 3,217 |
| 🥉 Seattle | $108,638 | 1,371 |
| San Francisco | $107,084 | 1,773 |
| Houston | $87,156 | 1,425 |
 
### 👥 Top 10 Customers by Sales
 
| Customer | T-Sales | T-Quantity |
|---|---|---|
| 🥇 Sean Miller | $25,043 | 50 |
| 🥈 Tamara Chand | $19,052 | 42 |
| 🥉 Raymond Buch | $15,117 | 71 |
| Tom Ashbrook | $14,595 | 38 |
| Adrian Barton | $14,473 | 73 |
 
### 📦 Top 10 Products by Sales
 
| Product | T-Sales |
|---|---|
| 🥇 Canon imageCLASS 2200 Advanced Copier | $61,599 |
| 🥈 Cisco TelePresence System EX90 | $22,638 |
| 🥉 Fellowes PB500 Electric Binding Machine | $27,453 |
| GBC DocuBind P400 Electric Binding System | $17,965 |
| GBC DocuBind TL300 Electric Binding System | $19,823 |
 
### 🏷️ Sales by Category & Sub-Category
 
| Category | Sub-Category | T-Sales | T-Quantity |
|---|---|---|---|
| **Furniture** | Chairs | $328,449 | 2,356 |
| | Tables | $206,966 | 1,241 |
| | Bookcases | $114,880 | 868 |
| | Furnishings | $91,705 | 3,563 |
| **Office Supplies** | Storage | $223,844 | 3,158 |
| | Binders | $203,413 | 5,974 |
| | Appliances | $107,532 | 1,729 |
| | Paper | $78,479 | 5,178 |
| | Supplies | $46,674 | 647 |
| | Art | $27,119 | 3,000 |
| | Envelopes | $16,476 | 906 |
| | Labels | $12,486 | 1,400 |
 
### 🚚 Sales by Ship Mode
 
| Ship Mode | T-Sales |
|---|---|
| Standard Class | $1,358,216 |
| Second Class | $459,194 |
| First Class | $351,428 |
| Same Day | $128,363 |
 
---
 
## 🗃️ Data Model
 
Built with **Power Pivot** using a **Star Schema**:
 
```
              ┌─────────────────┐
              │      Date       │
              │  Date           │
              │  Quarter        │
              │  Month Index    │
              │  Month Name     │
              │  Year           │
              └────────┬────────┘
                       │ 1
                       │
┌──────────────┐       │        ┌────────────────┐
│  Customers   │  1    ▼  *     │    Product     │
│              ├──►Transaction◄─┤                │
│ Customer ID  │               │  Product ID    │
│ Customer Name│               │  Category      │
│ Segment      │               │  Sub-Category  │
│ Country/City │               │  Product Name  │
│ State/Region │               └────────────────┘
└──────────────┘       │ *
                       │
                ┌──────┴──────┐
                │ DimShipping │
                │  Ship_ID    │
                │  Ship Mode  │
                └─────────────┘
```
 
### Tables Summary
 
| Table | Type | Rows | Key Columns |
|---|---|---|---|
| `Transaction` | ⭐ Fact | 9,994 | Order ID · Sales · Quantity · Discount · Profit |
| `Customers` | 👥 Dimension | — | Customer ID · Name · Segment · Region |
| `Product` | 📦 Dimension | — | Product ID · Category · Sub-Category · Name |
| `Date` | 📅 Dimension | — | Date · Quarter · Month · Year |
| `DimShipping` | 🚚 Dimension | — | Ship_ID · Ship Mode |
 
---
 
## 📊 Key KPIs at a Glance
 
```
┌──────────────────────────────────────────────────────────────┐
│                    BUSINESS SUMMARY                          │
├────────────────────────┬─────────────────────────────────────┤
│  💰 Total Sales        │  $2,297,201                         │
│  📦 Total Quantity     │  37,873 units                        │
│  💵 Total Profit       │  $286,397   (12.5% profit margin)   │
│  🏷️ Total Discount     │  $1,561                             │
│  📊 Total Transactions │  9,994 orders                        │
├────────────────────────┼─────────────────────────────────────┤
│  🏆 Top Customer       │  Sean Miller ($25,043)               │
│  🏆 Top City           │  New York City ($210,926)            │
│  🏆 Top Product        │  Canon imageCLASS 2200 ($61,599)    │
│  🏆 Top Category       │  Technology (highest avg sales)      │
│  🚚 Top Ship Mode      │  Standard Class ($1,358,216)         │
│  📅 Best Month         │  November ($352,461)                 │
└────────────────────────┴─────────────────────────────────────┘
```
 
---
 
## 🛠️ Tools & Technologies
 
| Tool | Usage |
|---|---|
| ![Excel](https://img.shields.io/badge/-Excel-217346?logo=microsoftexcel&logoColor=white&style=flat-square) | Dashboard, Pivot Tables, Charts |
| ![Power Pivot](https://img.shields.io/badge/-Power%20Pivot-0078D4?logo=microsoft&logoColor=white&style=flat-square) | Data model, Star Schema, DAX measures |
| ![Power Query](https://img.shields.io/badge/-Power%20Query-0EA5E9?style=flat-square) | ETL — data cleaning & transformation |
| ![Star Schema](https://img.shields.io/badge/-Star%20Schema-22C55E?style=flat-square) | Relational modeling across 5 tables |
 
---
 
## 📁 Project Structure
 
```
📦 Excel-Sales-Analysis/
├── 📊 Excel_Data_Analysis_Project.xlsx   ← Main Excel file
│   ├── 📋 Pivot Tables sheet             ← All analysis tables
│   └── 📊 Dashboard sheet               ← Interactive dashboard
├── 📸 screenshots/
│   ├── 01_Dashboard_Overview.png
│   ├── 02_Dashboard_Filtered.png
│   ├── 03_Pivot_Tables.png
│   ├── 04_Data_Model_PowerPivot.png
│   └── 05_Power_Query_Steps.png
└── 📄 README.md
```
 
---
 
## 🚀 How to Use
 
1. Download `Excel_Data_Analysis_Project.xlsx`
2. Open in **Microsoft Excel** (2016 or later — Power Pivot required)
3. Go to the **Dashboard** sheet
4. Use the **slicers** on the left to filter by Quarter, Category, or Sub-Category
5. All charts and KPI cards update **automatically**
6. Go to the **Pivot Tables** sheet to explore the raw analysis tables
> ⚠️ **Note:** If prompted to enable content or data connections, click **Enable** to allow Power Pivot to work correctly.
 
---
 
## 👤 About the Author
 
**Abd Elfatah Gaber Ebrahim**  
Data Analysis Student · ITI (Information Technology Institute) · Egypt 🇪🇬
 
<div align="center">
<a href="https://www.linkedin.com/in/abd-elfatah-gaber-ebrahim/"><img src="https://img.shields.io/badge/LinkedIn-Abd%20Elfatah%20Gaber-0A66C2?style=for-the-badge&logo=linkedin" alt="LinkedIn"/></a>
<a href="https://github.com/abd-elfatah-gaber"><img src="https://img.shields.io/badge/GitHub-abd--elfatah--gaber-181717?style=for-the-badge&logo=github" alt="GitHub"/></a>
<a href="https://mostaql.com/u/Abdelfatah26"><img src="https://img.shields.io/badge/Mostaql-Abdelfatah26-1abc9c?style=for-the-badge" alt="Mostaql"/></a>
<a href="https://khamsat.com/user/abd_elfatah_gaber26"><img src="https://img.shields.io/badge/Khamsat-abd__elfatah__gaber26-e67e22?style=for-the-badge" alt="Khamsat"/></a>
 
</div>
---
 
<div align="center">
⭐ <strong>If you found this project useful, please consider giving it a star!</strong> ⭐
 
<em>Built with ❤️ using Microsoft Excel · Power Pivot · Power Query</em>
 
</div>
 
