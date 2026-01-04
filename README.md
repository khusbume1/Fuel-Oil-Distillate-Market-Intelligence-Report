# Fuel Oil & Distillate Market Intelligence Pipeline

## Overview
This project builds an end-to-end market intelligence workflow for fuel oil and distillate markets using open-source data. The objective is to replicate how commodity analysts support trading desks by combining macro price regimes, weekly physical fundamentals, trade flows, and seasonality into actionable signals and market commentary.

The project emphasizes **interpretation and decision relevance**, not just data visualization.

---

## Markets Covered
- Crude oil (macro price regime context)
- Residual fuel oil (fuel oil balance proxy)
- Distillate (diesel/gasoil proxy with strong linkage to fuel oil via refinery yields and exports)

---

## Data Sources

### World Bank Pink Sheet
- Annual commodity prices (1960–present)
- Used to analyze long-term price regimes, volatility, and structural shocks

### U.S. Energy Information Administration (EIA)
- Weekly petroleum statistics via API
- Used to analyze:
  - Residual fuel oil stocks
  - Distillate stocks
  - Distillate imports and exports
  - Refinery utilization

---

## Methodology

The analysis follows a top-down market intelligence approach:

1. **Macro Context**
   - Identify long-term crude oil price regimes
   - Measure regime volatility and structural shocks

2. **Physical Market Balance**
   - Track weekly inventories and refinery utilization
   - Compute weekly builds/draws

3. **Trade-Flow Analysis**
   - Construct distillate net exports as an arbitrage pressure proxy

4. **Seasonality Normalization**
   - Build 5-year seasonal inventory baselines
   - Measure deviations from normal conditions

5. **Signal Generation**
   - Classify markets as Tight / Loose / Neutral
   - Generate a trader-style weekly market note

---

## Key Outputs

- Fuel oil & distillate balance dashboard
- Seasonal inventory deviation indicators
- Distillate net export (arb pressure) signal
- Auto-generated weekly market summary (Markdown)

Example output:

<img width="868" height="373" alt="image" src="https://github.com/user-attachments/assets/36ef90b3-0751-48ef-92b8-eb46b3aed902" />
<img width="877" height="373" alt="image" src="https://github.com/user-attachments/assets/8721c266-94ff-4257-a5b0-7fb4a1fa43a7" />
<img width="859" height="373" alt="image" src="https://github.com/user-attachments/assets/53869015-890a-4009-a671-94aececaf9d9" />
<img width="850" height="373" alt="image" src="https://github.com/user-attachments/assets/56e961fd-b970-404a-a115-3894ab3fd470" />

