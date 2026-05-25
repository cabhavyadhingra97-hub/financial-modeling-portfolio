# 📊 FP&A — Variance Analysis & Budget vs. Actuals

> **Financial Planning & Analysis dashboard: monthly budget vs. actuals with waterfall bridge and drill-down commentary**
> Full P&L variance analysis | Volume-Price-Mix decomposition | Dynamic Excel dashboard

---

## 🎯 Project Overview

| Parameter | Detail |
|-----------|--------|
| **Model Type** | FP&A — Budget vs. Actuals Variance Analysis |
| **Scope** | Full P&L (Revenue through Net Income) |
| **Granularity** | Monthly and YTD |
| **Decomposition** | Volume, Price, Mix variance |
| **Output** | Management dashboard + CFO-ready commentary |
| **Excel Features** | Dynamic charts, slicers, pivot tables, conditional formatting |

---

## 🏢 Business Context

A mid-size consumer goods company tracks 4 product segments across 3 regions. The FP&A model provides monthly actuals vs. budget visibility and identifies key drivers of variance to support management decision-making.

| Dimension | Detail |
|-----------|--------|
| **Segments** | Beverages, Snacks, Dairy, Packaged Foods |
| **Regions** | North, South, West |
| **Reporting Period** | Jan–Dec (full year) |
| **Reporting Cycle** | Monthly close + YTD |
| **Currency** | INR (₹) — amounts in Crores |

---

## 📋 FP&A Dashboard Structure

### Dashboard Tabs

| Tab | Content |
|-----|---------|
| **1. Executive Summary** | YTD P&L: Budget vs. Actuals; KPI scorecard; top 3 variances |
| **2. Revenue Variance** | Volume × Price × Mix waterfall; region-level split; segment drilldown |
| **3. COGS Variance** | Raw material, labour, overhead decomposition; purchase price variance |
| **4. Opex Variance** | S&M, R&D, G&A by function and cost centre |
| **5. EBITDA Bridge** | Waterfall from Budget EBITDA → Actual EBITDA |
| **6. Monthly Trend** | Rolling 12-month actuals vs. budget vs. prior year |
| **7. Assumptions & Drivers** | Macro inputs: CPI, FX, commodity prices |

---

## 📊 YTD P&L — Budget vs. Actuals (₹ Crores)

| Line Item | Budget | Actuals | Variance (₹) | Variance (%) | Assessment |
|-----------|:------:|:-------:|:------------:|:------------:|:----------:|
| **Revenue** | 1,850 | 1,792 | **(58)** | **(3.1%)** | ⚠️ Miss |
| COGS | (925) | (942) | **(17)** | **1.8%** | ⚠️ Higher |
| **Gross Profit** | **925** | **850** | **(75)** | **(8.1%)** | ❌ Below |
| Gross Margin | 50.0% | 47.4% | — | –260bps | ⚠️ |
| S&M | (280) | (265) | **15** | **5.4%** | ✅ Favorable |
| R&D | (120) | (118) | **2** | **1.7%** | ✅ On Track |
| G&A | (95) | (102) | **(7)** | **(7.4%)** | ⚠️ Overspend |
| **EBITDA** | **430** | **365** | **(65)** | **(15.1%)** | ❌ Miss |
| EBITDA Margin | 23.2% | 20.4% | — | –285bps | |
| D&A | (85) | (86) | **(1)** | **1.2%** | ✅ Neutral |
| **EBIT** | **345** | **279** | **(66)** | **(19.1%)** | ❌ Miss |
| Finance Costs | (42) | (44) | **(2)** | **4.8%** | |
| **PBT** | **303** | **235** | **(68)** | **(22.4%)** | |
| Tax (25%) | (76) | (59) | **17** | **22.4%** | |
| **PAT** | **227** | **176** | **(51)** | **(22.5%)** | ❌ |

---

## 📉 Revenue Variance — Volume-Price-Mix (VPM) Decomposition

### Total Revenue Variance: ₹(58) Cr

| Variance Component | Amount (₹ Cr) | Direction |
|-------------------|:-------------:|:---------:|
| **Volume Effect** | **(82)** | Unfavorable |
| **Price Effect** | **+38** | Favorable |
| **Mix Effect** | **(14)** | Unfavorable |
| **Total Revenue Variance** | **(58)** | Unfavorable |

### Volume Variance — By Segment

| Segment | Budget Vol (Mn units) | Actual Vol | Variance | ₹ Impact |
|---------|:---------------------:|:----------:|:--------:|:--------:|
| Beverages | 42.0 | 38.5 | (3.5) | (48) |
| Snacks | 28.0 | 29.8 | +1.8 | +18 |
| Dairy | 15.0 | 12.6 | (2.4) | (32) |
| Packaged Foods | 18.0 | 18.4 | +0.4 | +5 |
| **Total** | **103** | **99.3** | **(3.7)** | **(57)** |

### Price Variance — By Segment

| Segment | Budget ASP (₹) | Actual ASP | Variance | ₹ Impact |
|---------|:--------------:|:---------:|:--------:|:--------:|
| Beverages | 92 | 96 | +4 | +15 |
| Snacks | 148 | 155 | +7 | +21 |
| Dairy | 210 | 208 | (2) | (3) |
| Packaged Foods | 185 | 186 | +1 | +2 |
| **Total** | — | — | — | **+35** |

---

## 🏭 COGS Variance — Raw Material vs. Conversion

| COGS Component | Budget | Actual | Variance | Commentary |
|----------------|:------:|:------:|:--------:|-----------|
| Raw Material | (510) | (538) | **(28)** | Palm oil +22%, soybean +18% above budget |
| Direct Labour | (185) | (182) | **+3** | Efficiency gains in Snacks line |
| Manufacturing OH | (142) | (140) | **+2** | Energy costs below budget |
| Logistics | (88) | (82) | **+6** | Route optimization savings |
| **Total COGS** | **(925)** | **(942)** | **(17)** | Commodity inflation drove miss |

---

## 📈 EBITDA Waterfall Bridge

```
Budget EBITDA               430
+ Price Realization         +35
- Volume Shortfall          (57)
- Mix Shift (lower-margin)  (14)
- RM Inflation              (28)
+ Opex Savings              +10
- G&A Overspend             (7)
+ Other                     +6
────────────────────────────────
Actual EBITDA               365
Variance                    (65) | –15.1%
```

---

## 📅 Monthly Trend — Revenue (₹ Cr)

| Month | Budget | Actuals | Variance | Prior Year |
|-------|:------:|:-------:|:--------:|:----------:|
| Jan | 145 | 142 | (3) | 128 |
| Feb | 148 | 144 | (4) | 130 |
| Mar | 162 | 155 | (7) | 141 |
| Apr | 155 | 152 | (3) | 138 |
| May | 158 | 148 | (10) | 140 |
| Jun | 165 | 160 | (5) | 146 |
| Jul | 172 | 168 | (4) | 152 |
| Aug | 170 | 165 | (5) | 149 |
| **YTD** | **1,275** | **1,234** | **(41)** | **1,124** |

---

## 💡 CFO-Ready Management Commentary

### Revenue: ₹(58) Cr Unfavorable

Revenue underperformed budget by 3.1% driven primarily by volume shortfall in Beverages (–8.3%) and Dairy (–16%) due to supply chain disruptions in Q2 and intense competitive pressure in organized retail. This was partially offset by strong pricing realization (+₹38 Cr) following April price increase across Snacks and Beverages. YoY growth remains healthy at +12.3% vs. prior year.

### EBITDA: ₹(65) Cr Unfavorable (–15.1%)

EBITDA miss was driven by: (1) revenue volume shortfall flowing through at ~65% contribution margin = ₹(37) Cr impact; (2) commodity inflation — palm oil and soybean above budget by 18–22% adding ₹(28) Cr pressure; partially offset by (3) opex discipline in S&M (₹+15 Cr) due to campaign timing delays and logistics savings (₹+6 Cr). Management has initiated commodity hedging for H2 to de-risk exposure.

---

## 🛠️ Skills Demonstrated

- **FP&A Modelling:** Budget vs. actuals tracking, monthly close process, management reporting
- **Variance Analysis:** Volume-Price-Mix decomposition, EBITDA bridge/waterfall construction
- **Dashboard Design:** Excel dynamic charts, slicers, pivot tables, conditional formatting
- **Business Commentary:** CFO-ready narrative — quantified, cause-and-effect driven
- **Cost Analysis:** COGS decomposition (raw material, labour, overhead, logistics)
- **KPI Scorecarding:** Gross margin, EBITDA margin, revenue growth tracking vs. budget/PY

---

## 🔧 Tools Used

![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=flat&logo=microsoft-excel&logoColor=white)
![PowerBI](https://img.shields.io/badge/Power_BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![VBA](https://img.shields.io/badge/Excel_VBA-217346?style=flat&logo=microsoft-excel&logoColor=white)

**Methodology:** ICAI Management Accounting standards; CIMA variance analysis framework

---

*Part of [CA Bhavya Dhingra's Financial Modeling Portfolio](../../README.md)*
