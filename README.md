# 5-Year Network Expansion & 3-Statement Financial Model for a Retail Telecom Chain

> Extended practice build using a competition case by **Andrew Grigolyunovich, CFA, MFM** (FMWC). 
> The model and dashboard were built from scratch using the original narrative case and assumptions 
> table. 
---

## Overview

A 5-year monthly 3-statement financial model for **TeleKings Inc.**, a retail telecom chain operating 
1,000 stores across 26 cities. The model projects revenue, EBITDA, and full balance sheet position 
across 60 months while evaluating a structured store expansion plan and its financial implications.

**Tools:** Advanced Excel · 5-Year Financial Projections

---

## Business Question

> *How does opening one new store per month across 26 cities affect EBITDA, cash flow, and balance 
> sheet health — and at what point does adding stores start hurting the stores already there?*

---

## Model Architecture

### Store Expansion Engine
- 1,000 existing stores across 26 cities with 2025 actuals as the revenue baseline
- One new store opened per month, cycling alphabetically through all 26 cities
- Cycle restarts after ZeroDay Zone (Month 27) — two full alphabetical passes over 60 months
- New store revenue and rent benchmarked to the city average of existing stores
- Each new store adds 3 FTEs and triggers $100k CAPEX (2025 prices, inflation-adjusted)

### Cannibalization Model
- Population-per-store tracked monthly for all 26 cities
- When density falls at or below 10,000 people per store, a 20% revenue penalty activates
  across every store in that city simultaneously
- Six cities hit the threshold by Month 60 — three within the first year of expansion

### Revenue Model

| Stream | Margin | Basis |
|---|---|---|
| Device Sales | 10% gross margin | Monthly store average, inflation-adjusted |
| Accessory Sales | 70% gross margin | Monthly store average, inflation-adjusted |
| Mobile Plan Commissions | 100% margin | $100/activation (2025 prices) |

Seasonality applied monthly: January 80%, February 75%, December 150% of average.  
3% annual inflation compounds each January starting 2026 across all revenue and cost lines.

### Labor & OpEx
- Sales headcount grows by 3 FTEs per new store opened
- Hourly rate of $15.00 (2025) inflates annually
- Rent, other store costs, and G&A all step up with store count and inflation

### 3-Statement Integration
- Full P&L through to Net Income with EBITDA, EBIT, and EBT subtotals
- Balance sheet with working capital (AR at 50% of revenue, inventory at $92.5k/store 
  inflation-adjusted, AP at 100% of monthly expenses)
- Cash flow statement (indirect method) with revolving credit facility that auto-draws 
  when cash runs short and repays as soon as cash is available

### Debt Schedules
- **Senior fixed-rate loan** — $50M at 5.0%, 8yr remaining, equal monthly principal repayments
- **Variable subordinated debt** — $15M at SOFR+3.5%, 5yr remaining
- **Revolving credit facility** — up to $10M at 8.0%
- Interest calculated on opening monthly balance for all three facilities

### CAPEX & Depreciation
- New store CAPEX triggers on opening day, depreciated straight-line over 5 years from Month 2
- Existing PP&E depreciated over 3 years; intangibles amortized over 15 years

---

## Key Results

| Metric | Value |
|---|---|
| 5-Year Cumulative Revenue | $8.0B |
| 5-Year Total EBITDA | $620M |
| 5-Year Net Income | $403M |
| Ending Cash Balance (Month 60) | $267M |
| Store Count Growth | 1,000 → 1,060 |
| Cities Hitting Cannibalization Threshold | 6 of 26 |

### Recommendation: Proceed with Expansion — with Density Guardrails

The 60-month model projects $8.0B in cumulative revenue and $620M in total EBITDA. The revolver 
draws $7.6M in Month 1 to bridge early cash needs and is fully repaid by March 2026 with no 
further draws through Month 60. Six cities reach cannibalization density by Month 60, with three 
triggering in the first year — flagging clear markets where the expansion plan should pause in 
favor of underpenetrated cities.

---

## Excel Functions Used

`IF` · `SUMIFS` · `XLOOKUP` · `ANCHORARRAY` · `EOMONTH` · `INDEX/MATCH` · `OFFSET` · 
`COUNTA` · `DATE FUNCTIONS`

---

## About This Build

This model was built as an extended practice exercise using a competition case by 
**Andrew Grigolyunovich, CFA, MFM** for the **Financial Modeling World Cup** — a global 
competition where participants build financial models under timed conditions. The originating 
materials included a narrative case description and assumptions and original store table. The 
model and dashboard were built from scratch. Accuracy was verified against 25 official 
FMWC validation questions.

*Part of the [Alicia Bruce Data & Financial Analytics Portfolio](https://www.notion.so/Data-Financial-Analytics-Portfolio-323b743fecb880c49f67d0ada9312832)*
