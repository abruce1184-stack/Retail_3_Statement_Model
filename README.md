# TeleKings Inc. — 5-Year Network Expansion & Financial Projection Model

**Competition Case by Andrew Grigolyunovich, CFA, MFM. | Financial Modeling World Cup (FMWC)**

---

## Tools
Advanced Excel · 5-Year Financial Projections

## Industry
Retail | Multi-Store Network | Telecom

## Projection
60 months · Jan 2026 – Dec 2030

---

## The Business Problem

TeleKings operates 1,000 retail locations selling mobile devices, accessories, and mobile plan subscriptions. Management needed a 60-month 3-statement projection to evaluate a structured expansion plan opening one new store per month, cycling alphabetically through 26 cities. The key complication: once a city reaches a population-per-store density below 10,000 people, new stores cannibalize revenue from every existing store in that market. The model had to quantify exactly when that threshold hits and what it costs.

---

## What the Model Does

- **Store expansion engine** — city-by-city store count schedule with one new store opening per month across 26 markets, cycling alphabetically and restarting after ZeroDay Zone (Month 27). New store revenue and rent are benchmarked to the city average of existing stores.
- **Cannibalization model** — when population per store in a city falls at or below 10,000, a 20% revenue penalty activates across every store in that market simultaneously. Six cities hit this threshold by Month 60, creating a natural saturation ceiling for the expansion plan.
- **Revenue model** — three streams (device sales, accessory sales, mobile plan commissions) with month-level seasonality (Jan 80%, Feb 75%, Dec 150%) and 3% annual inflation compounding each January starting 2026.
- **Labor & OpEx** — sales headcount grows by 3 FTEs per new store; hourly rates inflate annually; rent, other store costs, and G&A all step up with store count and inflation.
- **3-statement integration** — full P&L through to Net Income, balance sheet with working capital (AR at 50% of revenue, inventory at $92.5k/store inflation-adjusted, AP at 100% of monthly expenses), and a cash flow statement with a revolving credit facility that auto-draws when cash runs short and repays as soon as cash is available.
- **Debt schedules** — senior fixed-rate loan ($50M, 5%, 8yr), variable-rate subordinated debt ($15M, SOFR+3.5%, 5yr), and a $10M revolver — all with interest calculated on opening monthly balance and equal principal repayments.
- **CAPEX & depreciation** — new store CAPEX of $100k (2025 prices, inflation-adjusted) triggers on opening day, depreciated straight-line over 5 years starting Month 2; existing PP&E depreciates over 3 years, intangibles over 15.

---

## Key Outputs

**Expansion is financially sound — with clear density limits to monitor**

The 60-month model projects $8.0B in cumulative revenue and $620M in total EBITDA across the expansion period. Store count grows from 1,000 to 1,060 locations and ending cash reaches $267M. Six cities reach cannibalization density by Month 60 (with three triggering in the first year). The revolver draws $7.6M in Month 1 to bridge early cash needs and is fully repaid by March 2026 with no further draws through Month 60.

---

## Excel Functions Used

`IF` · `SUMIFS` · `XLOOKUP` · `ANCHORARRAY` · `EOMONTH` · `INDEX/MATCH` · `OFFSET` · `COUNTA` · `DATE FUNCTIONS`

---

## Download



---

## Context About This Build

This model was built as an extended practice exercise using a Financial Modeling World Cup competition case authored by Andrew Grigolyunovich, CFA, MFM. The originating materials included a narrative case description and assumptions and original store table. The model and dashboard were built from scratch. Accuracy was verified against 25 official FMWC validation questions.

---

*Synthetic data — built for portfolio demonstration purposes only.*
