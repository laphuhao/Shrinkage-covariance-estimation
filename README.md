# Non-linear Shrinkage for Portfolio Optimization on the Vietnamese Stock Market

> **Published:** Proceedings of National Scientific Conference, Academy of Finance, 2024, pp. 384–397

---

## 📌 Overview
This research evaluates the effectiveness of **Non-linear Shrinkage covariance matrix estimation** (Ledoit & Wolf, 2020) for portfolio optimization in the context of high-dimensional data and the COVID-19 pandemic on the Vietnamese stock market (HOSE).

---

## 🎯 Motivation
Traditional covariance matrix estimation methods become unstable when the number of assets is large relative to observations. This study addresses that limitation by applying non-linear shrinkage techniques, which adjust eigenvalues of the sample covariance matrix using **Kernel density estimation** and **Hilbert transform**.

---

## 🗂️ Data & Methodology

| | Details |
|---|---|
| **Market** | Ho Chi Minh Stock Exchange (HOSE) |
| **Universe** | 370–407 listed stocks |
| **In-sample** | Jan 2019 – Dec 2019 |
| **Out-of-sample** | Jan 2020 – Dec 2023 (COVID-19 period) |
| **Objective** | Global Minimum Variance Portfolio (GMVP) |
| **Backtesting** | Rolling-Horizon (weekly rebalancing) |

---

## ⚙️ Methods Compared

| Method | Description |
|---|---|
| **Non-linear Shrinkage** | Analytical nonlinear eigenvalue adjustment (Ledoit & Wolf, 2020) |
| **LShrIM** | Linear shrinkage toward identity matrix (Ledoit & Wolf, 2004) |
| **LShrSI** | Linear shrinkage toward single-factor matrix (Ledoit & Wolf, 2003) |
| **VN-Index** | Market benchmark |

---

## 📊 Results

| Metric | Non-linear Shrinkage | LShrIM | LShrSI | VN-Index |
|---|---|---|---|---|
| Annual Return | **11.92%** | 11.32% | 7.11% | 3.97% |
| Volatility | **7.70%** | 7.93% | 11.56% | 21.70% |
| Sharpe Ratio | **1.50** | 1.39 | 0.65 | 0.051 |
| Max Drawdown | -17.14% | **-15.26%** | -34.93% | — |
| Win Rate | **57.1%** | 56.4% | 56.4% | 40.37% |
| Alpha | **6.93%** | 6.30% | 2.41% | — |

---

## 🔑 Key Findings

- ✅ Non-linear Shrinkage **outperforms all benchmarks** across return, risk, and Sharpe ratio
- ✅ **Lower portfolio turnover** (9.25%/week vs LShrIM 11.5%/week), reducing transaction costs
- ✅ **Robust during COVID-19 market stress** — volatility 2.8x lower than VN-Index
- ✅ Higher Alpha (6.93%) confirms consistent risk-adjusted outperformance over CAPM expectations

---

## 🛠️ Tools & Libraries

```python
Python · NumPy · Pandas · SciPy · statsmodels · matplotlib
```

---

## 📄 Publication

> Nguyen Minh Nhat, **La Phu Hao**, Nguyen Ngoc Huy, Nguyen Thanh Viet.
> *"Evaluating The Effectiveness Of The Non-linear Shrinkage Estimator In The Context Of High-dimensional Data And The COVID-19 Pandemic On The Vietnamese Stock Market"*.
> Proceedings of National Scientific Conference, Academy of Finance, 2024, pp. 384–397.
> 📘 [Finance Publishing House](https://fph.gov.vn)

---

## 👤 Author
**La Phu Hao** - Ho Chi Minh University of Banking
[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?logo=linkedin)](https://linkedin.com/in/laphuhao)
