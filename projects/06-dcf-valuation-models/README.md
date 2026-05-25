# 📉 DCF Valuation Models — Jazz Pharma & Steel Dynamics (STLD)

> **Two-company DCF study demonstrating cross-sector valuation: Pharma vs. Cyclical Industrials**
> Jazz Pharma: WACC 9.88% | STLD: Football field valuation | Combined 3-sheet Excel model

---

## 🎯 Project Overview

| Parameter | Detail |
|-----------|--------|
| **Companies** | Jazz Pharmaceuticals (JAZZ) + Steel Dynamics Inc. (STLD) |
| **Model Type** | Discounted Cash Flow (DCF) — Unlevered FCFF |
| **Valuation Methods** | DCF, EV/EBITDA, EV/Revenue, P/E Comparable Companies |
| **WACC (Jazz Pharma)** | **9.88%** |
| **Football Field** | Yes — 5 methodologies compared |
| **Excel Sheets** | 3 per company (6 total) |
| **Key Output** | Intrinsic value vs. market price comparison |

---

## 🏢 Company Profiles

### Jazz Pharmaceuticals (NASDAQ: JAZZ)

| Parameter | Value |
|-----------|------:|
| Sector | Specialty Pharmaceuticals |
| Revenue (LTM) | $3,660M |
| EBITDA (LTM) | $1,240M |
| EBITDA Margin | 33.9% |
| Net Debt | $4,820M |
| Shares Outstanding | 60.3M |
| Market Price (as of model) | $126 |

### Steel Dynamics Inc. (NASDAQ: STLD)

| Parameter | Value |
|-----------|------:|
| Sector | Steel Manufacturing (Cyclical Industrial) |
| Revenue (LTM) | $18,400M |
| EBITDA (LTM) | $3,850M |
| EBITDA Margin | 20.9% |
| Net Debt | $2,340M |
| Shares Outstanding | 152.4M |
| Market Price (as of model) | $108 |

---

## 📐 Model Architecture

### Jazz Pharma — 3-Sheet Model

| Sheet | Content |
|-------|---------|
| **Sheet 1: Historical & Projections** | 5-year actuals + 5-year forecast; revenue drivers (Oxybate franchise, Epidiolex, pipeline); segment-level margin assumptions |
| **Sheet 2: WACC & DCF** | Beta regression, risk-free rate, ERP, cost of debt, WACC calculation; FCFF projection; terminal value (Gordon Growth); bridge to equity value |
| **Sheet 3: Comparable Companies & Football Field** | 8-company peer set; EV/EBITDA, EV/Revenue, P/E multiples; football field chart |

### Steel Dynamics — 3-Sheet Model

| Sheet | Content |
|-------|---------|
| **Sheet 1: Historical & Projections** | Steel cycle awareness; volume + price drivers; scrap cost model; segment split (Steel, Metals Recycling, Steel Fabrication) |
| **Sheet 2: WACC & DCF** | Higher beta for cyclicality; mid-cycle EBITDA normalization; normalized DCF vs. peak DCF |
| **Sheet 3: Comparable Companies & Football Field** | Nucor, Commercial Metals, US Steel; industry EV/EBITDA; cycle-adjusted valuation |

---

## 📊 Jazz Pharma — DCF Deep Dive

### Revenue Projections

| Year | Revenue ($M) | Growth | EBITDA ($M) | Margin |
|------|:-----------:|:------:|:-----------:|:------:|
| FY23A | 3,660 | — | 1,240 | 33.9% |
| FY24E | 3,920 | 7.1% | 1,370 | 35.0% |
| FY25E | 4,210 | 7.4% | 1,500 | 35.6% |
| FY26E | 4,480 | 6.4% | 1,610 | 35.9% |
| FY27E | 4,680 | 4.5% | 1,700 | 36.3% |
| FY28E | 4,820 | 3.0% | 1,760 | 36.5% |
| **Terminal** | — | **3.0% (g)** | — | — |

### WACC Calculation

| Component | Value |
|-----------|------:|
| Risk-Free Rate (10Y UST) | 4.28% |
| Equity Risk Premium | 5.50% |
| Relevered Beta | 0.98 |
| **Cost of Equity (CAPM)** | **9.67%** |
| Pre-tax Cost of Debt | 6.80% |
| Tax Rate | 12.5% (IP holding structure) |
| After-tax Cost of Debt | 5.95% |
| Weight of Equity | 52% |
| Weight of Debt | 48% |
| **WACC** | **9.88%** |

### FCFF & DCF Output

| Year | EBITDA | D&A | EBIT | Tax | NOPAT | + D&A | - Capex | - ΔNWC | FCFF | PV |
|------|:------:|:---:|:----:|:---:|:-----:|:-----:|:-------:|:------:|:----:|:--:|
| FY24E | 1,370 | 420 | 950 | 119 | 831 | 420 | (280) | (65) | 906 | 824 |
| FY25E | 1,500 | 440 | 1,060 | 133 | 927 | 440 | (295) | (70) | 1,002 | 829 |
| FY26E | 1,610 | 455 | 1,155 | 144 | 1,011 | 455 | (305) | (72) | 1,089 | 820 |
| FY27E | 1,700 | 468 | 1,232 | 154 | 1,078 | 468 | (315) | (68) | 1,163 | 796 |
| FY28E | 1,760 | 478 | 1,282 | 160 | 1,122 | 478 | (322) | (65) | 1,213 | 754 |
| **TV (g=3%)** | — | — | — | — | — | — | — | — | **17,846** | **11,093** |
| **EV** | — | — | — | — | — | — | — | — | — | **15,116** |
| Less: Net Debt | — | | | | | | | | | **(4,820)** |
| **Equity Value** | — | | | | | | | | | **$10,296M** |
| **Per Share** | — | | | | | | | | | **$170.7** |

---

## 🎯 Football Field — Jazz Pharma

```
Method                     Low      Base     High
─────────────────────────────────────────────────
DCF (WACC ±1%)           142      171      205
EV/EBITDA (11–14x)       148      163      185
EV/Revenue (3.5–5.0x)   130      155      187
P/E Comp. (12–18x)       132      151      173
52-Week Range             97      —        148
─────────────────────────────────────────────────
Market Price                       $126
Implied Upside                    +35%
```

---

## 🏭 Steel Dynamics — Cyclical DCF Key Findings

| Metric | Peak Cycle | Normalized (Mid-Cycle) |
|--------|:----------:|:---------------------:|
| EBITDA ($M) | 3,850 | 2,400 |
| WACC | 10.2% | 10.2% |
| DCF Value (per share) | $138 | $94 |
| Market Price | $108 | $108 |
| Premium / (Discount) | +28% premium | –13% discount |

**Key Insight:** Mid-cycle normalized DCF ($94) suggests market is pricing STLD at peak cycle earnings — classic cyclical valuation trap. Recommended using EV/Replacement Cost and through-the-cycle EBITDA for appropriate positioning.

---

## 🔍 Comparable Company Analysis — Jazz Pharma

| Company | EV/EBITDA | EV/Rev | P/E | NTM Rev Growth |
|---------|:---------:|:------:|:---:|:--------------:|
| **Jazz Pharma (JAZZ)** | **9.4x** | **3.2x** | **10.1x** | **7%** |
| Supernus Pharma | 11.2x | 3.8x | 12.4x | 5% |
| Intra-Cellular Therapies | 28.4x | 9.2x | NM | 28% |
| Prestige Consumer | 10.6x | 3.4x | 14.2x | 3% |
| Amneal Pharma | 8.1x | 1.2x | NM | 6% |
| UCB (Belgium) | 12.4x | 3.6x | 18.1x | 9% |
| **Peer Median** | **11.5x** | **3.6x** | **13.3x** | **6%** |
| **Implied Jazz Value** | **$170** | **$158** | **$151** | — |

---

## 🛠️ Skills Demonstrated

- **DCF Modelling:** Unlevered FCF, WACC, terminal value (Gordon Growth + Exit Multiple)
- **Cross-Sector Valuation:** Pharma IP-driven vs. cyclical industrial — different normalization approaches
- **Beta & WACC:** Unlevering/relevering beta, tax-adjusted cost of debt, capital structure sensitivity
- **Comparable Company Analysis:** Peer selection, multiple calculation, implied value triangulation
- **Football Field Visualization:** Multi-method valuation range chart in Excel
- **Cyclical Adjustment:** Mid-cycle vs. peak EBITDA normalization for industrials

---

## 🔧 Tools Used

![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=flat&logo=microsoft-excel&logoColor=white)
![Bloomberg](https://img.shields.io/badge/Bloomberg_Terminal-000000?style=flat&logo=bloomberg&logoColor=white)
![SEC](https://img.shields.io/badge/SEC_EDGAR-003087?style=flat&logoColor=white)

**Data Sources:** SEC 10-K/10-Q filings (JAZZ, STLD), Bloomberg consensus estimates, Damodaran beta database, Federal Reserve (risk-free rate)

---

*Part of [CA Bhavya Dhingra's Financial Modeling Portfolio](../../README.md)*
