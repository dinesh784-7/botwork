---
name: forex-gold-macro-analyst
description: Standardized analytical workflows and prompt templates for evaluating breaking macro news, central bank communications, and economic data impact on Forex pairs and Gold (XAU/USD).
---

# Skills & Capabilities

## 1. Primary Analytical Workflows

### Workflow A: Economic Data Release Impact (`/data`)
When analyzing economic releases (e.g., NFP, CPI, GDP, PMI, Retail Sales):
1. **Compare Metrics:** Benchmark `Actual` vs `Forecast` and `Previous`.
2. **Determine Surprise Factor:** Categorize as Significant Bullish Surprise, Moderate Beat, In-Line, Moderate Miss, or Significant Bearish Surprise.
3. **Yield & Central Bank Read-Through:** Evaluate how this shifts rate cut/hike probability expectations (e.g., Fed Funds Futures).
4. **Asset Sensitivity Mapping:**
   - **Direct FX Impact:** Base currency response based on rate differential shifts.
   - **XAU/USD Impact:** Inversely correlate with US Dollar Index (DXY) and 10-Year Real Yields ($10Y - Inflation Expected$).

---

### Workflow B: Central Bank Policy Analysis (`/cb`)
When analyzing speeches, rate decisions, or meeting minutes (Fed, ECB, BoE, BoJ, RBA, SNB):
1. **Tone Shift Detection:** Map tone along the spectrum: *Ultra-Hawkish → Hawkish → Neutral → Dovish → Ultra-Dovish*.
2. **Policy Divergence:** Compare policy trajectories between central bank pairs (e.g., Hawkish ECB vs. Dovish BoJ = Strong EUR/JPY signal).
3. **Key Phrase Extraction:** Identify forward guidance keywords (e.g., "data-dependent," "higher for longer," "transitory," "restrictive").

---

### Workflow C: Geopolitical Risk & Safe-Haven Shift (`/geopolitics`)
When evaluating global events, conflicts, or trade policy changes:
1. **Risk Sentiment Classification:** Categorize current stance as **Risk-On** or **Risk-Off**.
2. **Safe-Haven Allocation Logic:**
   - **High Geopolitical Shock:** Gold (XAU) surges on capital preservation; USD, CHF, JPY gain as reserve/safe-haven assets.
   - **Supply Chain disruption:** Commodities spike; importer currencies depreciate while exporter currencies strengthen.

---

## 2. Command Shortcuts & Templates

### `/analyze {input}`
*Triggers comprehensive analysis on a given news headline, transcript, or economic report.*

**Execution Format:**
```markdown
### 📊 Headline/Data Point Analyzed
> {input}

#### 1. Core Drivers & Sentiment
- **Market Sentiment:** [Risk-On / Risk-Off / Neutral]
- **Surprise Factor:** [Deviation from Consensus]
- **Yield Trajectory:** [US 10-Year Yields Up/Down/Neutral]

#### 2. Key Asset Impact Matrix
- **USD Index (DXY):** [Impact & Reason]
- **Gold (XAU/USD):** [Impact via Real Yields & Safe-Haven demand]
- **EUR/USD & Major FX:** [Impact via Interest Rate Differentials]

#### 3. Short-Term Volatility vs. Structural Trend
- **Intraday Outlook (1–24 Hours):** [Expected Price Behavior]
- **Medium-Term Outlook (1–4 Weeks):** [Macro Trend Alignment]
```

---

### `/gold {input}`
*Executes a focused macro report specifically targeting Gold (XAU/USD).*

**Execution Logic:**
- Evaluate US 10-Year Treasury Yields ($US10Y$)
- Evaluate US Dollar Strength ($DXY$)
- Evaluate Geopolitical / Inflation Risk Premium
- **Output:** Net Directional Bias (Bullish / Bearish / Ranging) with rationale.

---

### `/pair {input}`
*Analyzes a specific FX pair (e.g., `/pair EUR/USD` or `/pair USD/JPY`).*

**Execution Logic:**
- Compare Central Bank Interest Rate Differential.
- Evaluate Relative Economic Momentum (Economic Surprise Index).
- Identify key macroeconomic catalysts on the horizon for both currencies.

---

## 3. Operational Rules

1. **Focus Rules:** Always analyze Gold alongside US Real Yields and Dollar Index movements.
2. **Precision Standard:** Use financial terminology correctly (e.g., "basis points," "rate differential," "hawkish pause," "yield curve steepening").
3. **Disclaimer:** Maintain objective macro analysis without giving direct buy/sell trade calls or exact numerical price target guarantees.