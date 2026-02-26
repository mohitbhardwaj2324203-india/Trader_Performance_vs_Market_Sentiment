**Regime-Based Performance & Strategy Optimization**
📌 Project Overview

This project analyzes trader behavior across different market sentiment regimes (Fear, Greed, Extreme Greed, Neutral) using historical transaction data aligned with daily sentiment classification.

The objective is to evaluate how sentiment influences:

Profitability (PnL)

Win rate

Leverage usage

Trade frequency

Behavioral bias (Long/Short)

Trader segmentation performance

The final goal is to derive actionable trading strategy recommendations.

🧩 Dataset Description
1️⃣ Trader Dataset

Contains transactional trade-level data including:

Account

Execution Price

Size (USD & Tokens)

Closed PnL

Direction

Timestamp

Start Position

2️⃣ Sentiment Dataset

Daily market sentiment classification:

Fear

Greed

Extreme Greed

Neutral

🛠 Methodology
🔹 Part A — Data Preparation

Converted timestamps to daily format

Merged trader data with sentiment classification

Removed unmatched sentiment dates

Created key metrics:

Daily PnL per trader

Win rate

Average trade size

Trade frequency

Leverage proxy

Long/Short distribution

🔹 Part B — Sentiment Regime Analysis

We compared performance across sentiment regimes:

Average Daily PnL

Win Rate

Trade Frequency

Leverage Usage

Behavioral Direction Bias

We further segmented traders into:

High vs Low Leverage

Frequent vs Infrequent Traders

📈 Key Findings
1️⃣ Fear Regime Generates Highest Profitability

Fear periods show the highest average Daily PnL despite lower win rates, indicating larger winning trades during volatility expansion.

2️⃣ Extreme Greed Increases Risk Exposure

Leverage usage peaks during Extreme Greed but profitability does not scale proportionally, suggesting overconfidence-driven risk.

3️⃣ Overtrading Reduces Performance

Infrequent traders outperform frequent traders in most regimes, especially during Fear and Neutral conditions.

📊 Segmentation Insights

Low leverage traders outperform high leverage traders during Fear regimes.

High leverage performs better during Greed regimes (trend continuation).

Infrequent traders consistently achieve better average PnL than frequent traders.

🎯 Strategy Recommendations
✅ Strategy 1 — Fear Regime Discipline

Increase participation during Fear regimes with controlled leverage. Focus on volatility-driven setups rather than aggressive overtrading.

✅ Strategy 2 — Greed Regime Trend Exploitation

Apply controlled leverage scaling during Greed phases for trend continuation strategies while limiting excessive exposure.

✅ Strategy 3 — Activity Optimization

Adopt selective participation. Reduce trade frequency during Neutral and Extreme Greed environments to improve risk-adjusted returns.

📊 Tools & Technologies

Python

Pandas

NumPy

Seaborn / Matplotlib

SciPy

Scikit-Learn 
Author

Mohit
Junior Data Scientist Candidate
