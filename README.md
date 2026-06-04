<div align="center">

# 🏗️ RES Global F&C — MIS Dashboard
### Real Estate Services | Global Facilities & Construction | Business Execution Team

**Portfolio Project by [Amit Kumar](mailto:amitjsr831003@gmail.com) — Data Analyst**

</div>

---

## 📌 Project Overview

A fully automated **Management Information System (MIS)** built in Excel for the **Real Estate Services — Global Facilities & Construction (F&C)** Business Execution Team. This workbook enables senior APAC leadership to track the entire F&C project portfolio with live KPIs, Capex/Opex budget variance analysis, country-level scorecards, and executive-level reporting — all from a **single source of truth**.

> Simulates exactly what a **Data Analytics Officer** would deliver to the APAC Business Execution Team Lead for strategic and reporting submissions to Global F&C senior leadership.

---

## 🖼️ Dashboard Screenshots

### 🏠 Cover Sheet — Navigation Hub
> Entry point with analyst info, report metadata, and clickable navigation to all 5 dashboards.

![Cover Sheet](screenshots/final/final_cover.png)

---

### 📊 Executive Summary — Senior Leadership View
> KPI tiles showing total active projects, full-year budget, YTD spend, variance %, and on-time delivery rate. Includes Budget vs Actual bar chart and project status breakdown with risk flags.

![Executive Summary](screenshots/final/final_exec.png)

---

### 🏗️ Project Tracker — Full Portfolio Operations View
> All 12 active APAC F&C projects with auto-calculated variance, variance %, completion data bars, and **RAG (🟢 Green / 🟡 Amber / 🔴 Red)** status auto-assigned by threshold rules.

![Project Tracker](screenshots/final/final_tracker.png)

---

### 💰 Budget & Cost MIS — Capex / Opex Tracking
> Month-by-month Capex and Opex tracking with variance heat map (red = over budget, green = under), savings column, and a 12-month trend line chart comparing budget vs actual.

![Budget & Cost MIS](screenshots/final/final_budget.png)

---

### 📈 Performance Analysis — Category & Country Deep-Dive
> Dual analysis: (1) by project category (Interior Fit-out, New Build, MEP, Space Planning, Renovation) and (2) by country — with efficiency status flags and a pie chart showing spend distribution.

![Performance Analysis](screenshots/final/final_perf.png)

---

### 🌏 APAC Regional View — Country Scorecard
> 10-country APAC scorecard ranking each country on a composite **Country Score** (budget efficiency × completion rate), with automated RAG status and a horizontal bar chart for visual comparison.

![APAC Regional View](screenshots/final/final_apac.png)

---

### 📋 Data Repository — Single Source of Truth
> Master data layer with 12 project records and 60 rows of monthly financial data (12 months × 5 regions). All 5 dashboards pull exclusively from this sheet via SUMIF/COUNTIF formulas.

![Data Repository](screenshots/final/final_data.png)

---

## 💡 Key Insights Generated

### 1. 📦 Portfolio Health
- **12 active projects** across 10 APAC countries with a combined approved budget of **$32.4M**
- **6 projects (50%) are In Progress**, 3 Completed, 2 in Planning, 1 On Hold
- YTD spend of **$18.7M = 58% budget utilization** — healthy pacing for FY 2024-25
- Tokyo Data Centre (P003) is the **only over-budget project** at +$150K (+3.6%), flagged 🔴 RED

### 2. 💸 Budget & Variance Analysis
- **FY Total Capex variance is +3.2%** — slightly over budget, driven by Japan MEP project
- **Thailand (P005 Bangkok Hub)** is On Hold with only 20% spend — $2.48M undeployed capital
- Monthly Capex trend shows a **mid-year peak (Aug-Oct)** with stabilization in Q4
- **$1.54M in total savings** identified across the portfolio from under-budget projects

### 3. 🏆 Category Performance
- **Interior Fit-out** is the most active category (4 projects, $5.65M budget) — all Under Budget ✅
- **New Build** carries the highest risk — 2 Critical projects (Seoul, Bangalore) totalling $13M
- **MEP** projects show highest cost overrun tendency — Tokyo DC exceeded budget by 3.6%
- **Renovation** category has 100% Green RAG status — lowest risk category

### 4. 🌏 APAC Country Rankings
- **India leads** with 3 projects totalling $11.5M budget — highest portfolio concentration
- **Japan** shows 0% spend efficiency on its single project (completed, over budget)
- **Malaysia & Australia** are top performers — both completed on/under budget with 100% completion
- **South Korea (Seoul Tech Campus)** is flagged highest risk — $5.5M Critical project at only 2% completion

### 5. 📅 Monthly Opex Trends
- Opex remained stable across all months (within 5-8% of budget) — strong cost discipline
- **India and Japan** are the highest Opex-consuming regions month-on-month
- Efficiency Score peaked in **Nov-24 and Jan-25** — aligns with project milestone completions

---

## 🗂️ Workbook Structure

```
RES_FC_MIS_Dashboard_AmitKumar.xlsx
│
├── 🏠 Cover                   ← Navigation hub, analyst details, report metadata
├── 📊 Executive_Summary       ← KPI tiles + bar chart + status breakdown (senior leadership)
├── 🏗️ Project_Tracker         ← Full portfolio, RAG status, variance, completion data bars
├── 💰 Budget_Cost_MIS         ← Monthly Capex/Opex, variance heatmap, trend line chart
├── 📈 Performance_Analysis    ← By category + by country, efficiency flags, pie chart
├── 🌏 APAC_Regional           ← Country scorecard, composite score, ranking chart
└── 📋 Data_Repository         ← Master data source (all dashboards pull from here)
```

---

## ⚙️ Technical Highlights

| Feature | Detail |
|---|---|
| **Live Formulas** | 621 formulas — SUMIF, COUNTIF, COUNTIFS, AVERAGEIF, IFERROR, nested IF |
| **Data Model** | Single source (Data_Repository) feeds all 5 dashboards — no duplicate data |
| **Charts** | BarChart (clustered), LineChart (trend), PieChart, Horizontal BarChart |
| **Conditional Formatting** | ColorScale (variance heatmap), DataBar (completion %), CellIs (RAG rules) |
| **RAG Automation** | Red/Amber/Green auto-assigned via IF threshold formulas on variance & completion |
| **Color Convention** | Blue = hardcoded inputs · Black = formula outputs (industry standard) |
| **Automation** | Entire workbook built programmatically with Python (openpyxl) |
| **Error Rate** | ✅ Zero formula errors across all 621 formulas (verified with LibreOffice recalc) |

---

## 💼 JD Alignment

| JD Requirement | This Project Delivers |
|---|---|
| Database Development & Maintenance | Data_Repository as scalable, normalized master data source |
| Data-Driven Decision Making | KPI tiles, RAG flags, variance thresholds, composite scoring |
| Data Visualization & Reporting | 5 dashboards · 4 chart types · conditional formatting |
| Stakeholder Reporting to Global Seniors | Executive Summary built specifically for C-suite/senior leadership view |
| Advanced Excel proficiency | 621 formulas, pivot-style summaries, professional formatting |
| APAC / Real Estate domain simulation | 10 APAC countries · F&C project categories · Capex/Opex split |
| Process Improvement & Simplification | Single source of truth eliminates manual copy-paste reporting |
| Proactive Analysis | Automated RAG flags surface at-risk projects without manual review |

---

## 🚀 How to Use

1. **Open** `RES_FC_MIS_Dashboard_AmitKumar.xlsx` in Microsoft Excel (2016 or later)
2. Navigate using the **Cover sheet** cards or the sheet tabs at the bottom
3. **Update project data** only in `Data_Repository` — all dashboards auto-refresh
4. **Add new projects**: append rows to the Project Master table (rows 3–14, extend formulas down)
5. **Update monthly financials**: edit the blue-highlighted input cells in `Budget_Cost_MIS`

> 💡 **Tip:** Press `Ctrl + Home` on any sheet to jump back to the top. Freeze panes are set on all analytical sheets so headers stay visible while scrolling.

---

## 🔧 Rebuild from Source

```bash
# Clone the repo
git clone https://github.com/yourusername/RES_FC_MIS.git
cd RES_FC_MIS

# Install Python dependency
pip install openpyxl

# Rebuild the workbook from scratch
python build_mis.py

# Recalculate and verify all formulas (requires LibreOffice)
python scripts/recalc.py RES_FC_MIS_Dashboard_AmitKumar.xlsx
```

---

## 📁 Repository Structure

```
RES_FC_MIS/
├── 📊 RES_FC_MIS_Dashboard_AmitKumar.xlsx   ← Main deliverable
├── 🐍 build_mis.py                           ← Python build script (openpyxl)
├── 📖 README.md                              ← This file
├── 📸 screenshots/
│   └── final/
│       ├── final_cover.png
│       ├── final_exec.png
│       ├── final_tracker.png
│       ├── final_budget.png
│       ├── final_perf.png
│       ├── final_apac.png
│       └── final_data.png
└── 🔧 scripts/
    ├── recalc.py                             ← Formula recalculation via LibreOffice
    └── office/soffice.py                     ← LibreOffice helper
```

---

## 👤 About the Author

<table>
<tr>
<td><b>Name</b></td><td>Amit Kumar</td>
</tr>
<tr>
<td><b>Role</b></td><td>Data Analyst | BI Developer | 5+ Years Experience</td>
</tr>
<tr>
<td><b>Location</b></td><td>Jamshedpur, Jharkhand, India</td>
</tr>
<tr>
<td><b>Email</b></td><td>amitjsr831003@gmail.com</td>
</tr>
<tr>
<td><b>Core Skills</b></td><td>Python · SQL · Power BI · Excel · PySpark · Tableau · Metabase · Power Automate</td>
</tr>
</table>

---

<div align="center">

*📌 This project is part of Amit Kumar's data analytics portfolio. Built to demonstrate real-world MIS reporting capability aligned with the Data Analytics Officer — RES F&C role.*

⭐ *If this project helped you, please give it a star!*

</div>
