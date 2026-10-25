# roadtoquantmf

A 25-week self-study plan for quantitative finance (November 2025 to May 2026) and the work for week 1. Weeks 2 to 25 have no work in this repo.

- `Overview.md`: the plan, in two versions one after the other. Each week has topics, free resources, a weekly project and LeetCode targets. The first version ties every week to an economics topic, the second adds a computing topic to most weeks (parallel, cluster, cloud, grid and GPU computing).
- `Week 1.md`: the week 1 checklist, all ticked.
- `notebooks/linear_algebra_basics.ipynb`: the week 1 project. It downloads one year of daily closes for NVDA, TSLA, SPY and QQQ with yfinance, computes daily returns and the annualised covariance matrix, and runs an eigen decomposition (PCA). In the saved run (249 trading days up to 2025-11-17) the first principal component explains 76.9% of the variance. It plots NVDA vs TSLA daily returns, the weights of the first component (`notebooks/week01_pca_weights.png`) and that component's cumulative return. The checklist mentions the first two eigenvectors, the notebook plots the first one only.

Stack: Python (the notebook was saved with 3.14), NumPy, pandas, matplotlib, yfinance.

## Run

```
pip install numpy pandas matplotlib yfinance jupyter
jupyter notebook notebooks/linear_algebra_basics.ipynb
```

The data comes from yfinance at run time, so it needs internet and the numbers change with the date.

Status: week 1 of 25 done, all committed on 2025-11-18. No commits since.
