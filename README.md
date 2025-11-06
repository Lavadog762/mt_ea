# mt_ea
Pattern Recognition Expert Advisor for Metatrader

Step 1: Install the EA

MT4:

Copy PatternMatchTrader_v15.mq4 into MQL4/Experts/

Restart MT4 or refresh the Navigator panel.

MT5:

Copy PatternMatchTrader_v15.mq5 (same file works, rename .mq5) into MQL5/Experts/

Restart MT5 or refresh the Navigator panel.

Step 2: Load Historical Data

Go to Tools → History Center.

Download the data for your symbol and timeframe (e.g., EURUSD, M5).

For MT5, tick data can be downloaded using the built-in history downloader.

Tip: For pattern matching, having at least 3–6 months of clean historical bars is sufficient. Longer history increases CPU load.

Step 3: Configure EA Inputs

Recommended starting settings:

Input	Suggested Value
BarsPerPattern	35
SimilarityThreshold	0.9
LookAheadBars	20
Step	5
HistoryLimit	1000
RiskPerTrade	0.01 (1% of equity)
MaxDailyLoss	0.02 (2%)
RiskRewardRatio	2.0
TrailingStopPercent	0.5
MA_Period	50
RSI_Period	14
RSI_BuyLevel / SellLevel	50
StartHourEST / EndHourEST	8 / 12
PreCloseBufferMinutes	5
