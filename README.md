# GRTUSDT 1-Minute Historical Kline Dataset

An institutional-grade, open-source archive of cleaned, standardized, and validated **1-minute intraday historical kline data** for **GRTUSDT** (Binance Spot).

---

## 📊 Dataset Specifications
- **Symbol:** `GRTUSDT`
- **Market:** Binance Spot
- **Timeframe:** 1 Minute (`1m`)
- **Total Months:** `71` months
- **Total Candles:** `3,055,966` 1-minute candles
- **Historical Range:** `2020-12-17 20:30:00` to `2026-10-10 23:59:00` (UTC)
- **Schema:** `timestamp, datetime_utc, open, high, low, close, volume, quote_volume, trade_count, taker_buy_volume, taker_buy_quote_volume`

---

## 🏛️ Directory Hierarchy
```text
GRTUSDT-Historical-Data/
├── README.md
└── 1m/
    └── <YYYY>/
        └── <MM>/
            └── GRTUSDT_1m_<YYYY-MM>.csv
```

---

## ⚡ 1-Line Pandas Stream Loader
Load any month directly from GitHub's raw CDN without cloning the repository:

```python
import pandas as pd

url = "https://raw.githubusercontent.com/parshant231234-eng/GRTUSDT-Historical-Data/main/1m/2026/10/GRTUSDT_1m_2026-10.csv"
df = pd.read_csv(url)
print(df.head())
```
