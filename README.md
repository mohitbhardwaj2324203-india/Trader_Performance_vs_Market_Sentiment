**Regime-Based Performance & Strategy Optimization**


📌 Project Overview

This project analyzes trader behavior across different market sentiment regimes (Fear, Greed, Extreme Greed, Neutral) using historical transaction data aligned with daily sentiment classification.

The objective is to evaluate how sentiment influences:

Profitability (PnL)

Win rate

Risk exposure (leverage proxy)

Trade frequency

Behavioral bias (Long/Short)

Trader segmentation performance

The final goal is to derive actionable trading strategy recommendations based on measurable performance differences.

🧩 Dataset Description
1️⃣ Trader Dataset

Trade-level historical data including:

Account

Execution Price

Size (USD & Tokens)

Closed PnL

Direction

Timestamp

Start Position

2️⃣ Sentiment Dataset

Daily Bitcoin market sentiment classification:

Fear

Greed

Extreme Greed

Neutral

🛠 Methodology
🔹 Part A — Data Preparation

Converted timestamps to daily format

Merged trader data with daily sentiment classification

Removed unmatched sentiment dates

Aggregated performance at daily trader level

Created key metrics:

Daily PnL per trader

Win rate

Average trade size

Trade frequency

Risk exposure proxy (calculated as trade size relative to starting position, since explicit leverage was not available in the dataset)

Long/Short distribution

🔹 Part B — Sentiment Regime Analysis

Performance was compared across sentiment regimes using:

Average Daily PnL

Win Rate

Trade Frequency

Risk Exposure

Behavioral Direction Bias

Traders were segmented into:

High vs Low Risk Exposure

Frequent vs Infrequent Traders

📈 Key Findings
1️⃣ Fear Regime Shows Highest Average PnL

Fear regimes demonstrate the highest average Daily PnL despite a relatively lower win rate.
This suggests that while fewer trades are profitable, winning trades tend to be larger during high-volatility periods.

2️⃣ Risk Exposure Performance Varies by Regime

During Fear, low-risk traders outperform high-risk traders.

During Greed, high-risk traders significantly outperform low-risk traders.

This indicates that aggressive positioning is rewarded during optimistic market phases, while defensive positioning performs better during uncertain environments.

3️⃣ Overtrading Reduces Profitability

Infrequent traders outperform frequent traders across most regimes, particularly during Fear and Neutral conditions.

This suggests that selective participation yields stronger profitability than continuous high-frequency activity.

📊 Segmentation Insights

Low risk exposure performs better during Fear regimes.

High risk exposure performs better during Greed regimes.

Infrequent traders consistently achieve higher average PnL compared to frequent traders.

🎯 Strategy Recommendations
✅ Strategy 1 — Defensive Mode During Fear

Reduce risk exposure and focus on high-conviction setups during Fear regimes to improve downside protection.

✅ Strategy 2 — Controlled Scaling During Greed

Increase exposure selectively during Greed regimes where higher risk strategies demonstrate stronger performance.

✅ Strategy 3 — Optimize Trade Frequency

Adopt a selective trading model. Reduce excessive trade frequency during Neutral and Extreme Greed conditions to improve risk-adjusted returns.

📊 Tools & Technologies

Python

Pandas

NumPy

Matplotlib / Seaborn

SciPy

Scikit-Learn

📂 Data Availability Note

The analysis was performed using the exact datasets provided in the assignment email.
Due to GitHub file size limitations (25MB upload restriction), the original raw datasets are not included in this repository.

The notebook is fully reproducible when the provided datasets are placed in the designated /data folder.

👤 Author

Mohit
Junior Data Scientist Candidate
