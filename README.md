# Nvidia-DCF-Comps
Built during an AmplifyME x CFA Institute Investment Banking Career Bootcamp in a timed challenge. Features a DCF analysis with a sensitivity table, a comps analysis, a table showcasing ratios and key metrics, and a discussion regarding the value of the company. Historical values, assumptions, and formatting were all provided. Results and analysis should be considered within the context of the simulation. 

(Screenshots and excel file may be published later. Awaiting permission to make sure the terms of service are violated.)

## Overview
This project is an equity valuation of NVIDIA (NVDA) built within a structured simulation environment. Historical financials, projected assumptions, and the income statement/balance sheet/cash flow statement framework were provided by the CFA Institute and AmplifyME. I was responsible for building the DCF model, trading comps analysis, financial ratios, sensitivity table, and the final valuation discussion.

## What I Built

**WACC Calculation** — Cost of equity via CAPM (risk-free rate, equity beta, equity risk premium), weighted average cost of debt from Nvidia's bond schedule, and capital structure weighting to arrive at a ~10.8% WACC

**Discounted Cash Flow** — 5-year projection of unlevered free cash flows (2027–2031), discount factors, NPV of projected FCFs, and terminal value using the perpetuity growth method (2% terminal growth rate)

**Comparable Company Analysis** — Enterprise value multiples for Nvidia and high/mean/median/low summary statistics to compare peer groups.

**Financial Ratios** — Profitability (gross margin, EBITDA margin, operating margin), liquidity (current ratio, quick ratio), activity (DSO, DPO), leverage (debt/equity, debt/capital, debt/EBITDA), and coverage (EBITDA/interest, (EBITDA−CapEx)/interest) across historical and projected periods

**Valuation Conclusion** — overvalued/undervalued assessment, written justification, and discussion of assumption limitations

## What Was Provided

The simulation template included pre-built historical financial statements (FY2023–FY2026), projected income statement and balance sheet drivers (revenue growth step-down, margin assumptions, working capital ratios, D&A, capex, tax rate escalation, etc.), and the three-statement model linking income statement, balance sheet, and cash flow statement. Comparable company market data, blended valuation analysis, and historical ratios were also provided.

## Key Findings

| Method | Implied Share Price | vs. Market ($171.24) |
|--------|-------------------:|---------------------|
| DCF (Perpetuity Growth) | $221.82 | +30% upside |
| EV/EBITDA Comps (FY1 Mean) | $212.17 | +24% upside |
| EV/Revenue Comps (FY1 Mean) | $135.45 | −21% downside |
| Current Market EV | $169.01 | ~at market |
| **Blended (25% each)** | **$184.61** | **+7.8% upside** |

Conclusion: Fairly valued to modestly undervalued. The DCF and EV/EBITDA comps both indicate meaningful upside, while EV/Revenue comps suggest downside. This reflects the tension between Nvidia's exceptional margins and what peer multiples would imply. The upside of this valuation is contingent on continued margin performance. 

## Assumptions I Would Change

Revenue growth: The 10 percentage point annual step-down (60% → 20%) is mechanical. A bottom-up revenue build using segment-level data and management guidance would produce more defensible projections.

Valuation weighting: DCF and EV/EBITDA better capture the actual economics of the business considering Nvidia's high gross profit margin. EV/Revenue does not capture that affect so it may be better to overweight other aspects of the valuation relative to this measure if we assume gross profit margins will continue to hold. 

Comp set: I would consider a different peer group for better comparability. For example TSMC is a foundry and Nvidia supplier, not a true comparable. A tighter peer set focused on high-performance data center exposure (AMD, Broadcom, Marvell) would improve the analysis.

## Model Structure

The model lives in a single Excel workbook with the following layout on the main worksheet:

Rows 9–42 — Income statement and drivers (historical + projected)
Rows 49–87 — Balance sheet and drivers
Rows 94–134 — Cash flow statement and drivers
Rows 136–157 — WACC calculation
Rows 161–191 — DCF, terminal value, equity bridge, and sensitivity table
Rows 196–225 — Trading comps and implied enterprise values
Rows 232–255 — Financial ratios and key metrics
Rows 258–275 — Valuation conclusion and discussion

## Tools & Sources

Microsoft Excel

CFA Institute & AmplifyME simulation platform
