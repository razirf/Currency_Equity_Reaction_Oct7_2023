# Currency_Equity_Reaction_Oct7_2023
"Analysis of currency and equity market reactions to the October 7, 2023 Middle East conflict using Python and financial data APIs."
# 💹 Currency & Equity Market Reaction – October 7, 2023 Conflict

**An event-driven financial analysis examining global and regional market responses to the October 7, 2023 Middle East conflict.**  
This project visualizes how currency pairs, major stock indices, and the Tehran Stock Exchange (TSE) reacted before and after the outbreak of the conflict.

---

## 🧭 Project Overview
This notebook investigates the **short-term market reaction** to the October 7, 2023 conflict.  
It studies how **global currencies** and **equity indices** responded around the event window and compares them with Iran’s **Tehran Stock Exchange (TSE)** performance.  

The aim is to identify how geopolitical uncertainty affects risk assets, safe havens, and regional markets through normalized comparative visualizations.

---

## 🎯 Objectives
1. Analyze how **geopolitical shocks** influence major currencies and stock indices.  
2. Compare **safe-haven behavior** (USD, Gold proxies) vs. **risk assets** (equities, emerging currencies).  
3. Assess whether the **Tehran Stock Exchange (TSE)** aligns with or diverges from global market trends.  
4. Visualize **before-and-after market patterns** across currencies and indices.

---

## 🧩 Datasets and Sources

| Category | Source | Symbol / Method |
|-----------|---------|----------------|
| **Global Indices & FX Rates** | Yahoo Finance (`yfinance`) | `DX-Y.NYB`, `CNYUSD=X`, `AEDUSD=X`, `SARUSD=X`, `IQDUSD=X`, `EURUSD=X`, `^GSPC`, `399001.SZ` |
| **Iranian Market Data** | `finpy_tse` | `Get_CWI_History` (TSE Index), `Get_USD_RIAL` (USD/IRR official rate) |
| **Date Conversion** | `jdatetime` | Jalali–Gregorian conversion |
| **Note** | `SYPUSD=X` (Syrian Pound) attempted, but data unavailable. |

---

## 🗓️ Event Window
```python
start = '2023-09-25'
end = '2023-10-13'
split_date = '2023-10-09'  # Separation between pre-/post-conflict data

