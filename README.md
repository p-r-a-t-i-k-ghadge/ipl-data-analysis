# 🏏 IPL Data Analysis | Python · Pandas · Seaborn

> End-to-end Exploratory Data Analysis of the Indian Premier League (2008–2024)
> built as a beginner-friendly Google Colab notebook.

---

## 📌 Project Overview

The Indian Premier League is one of the most data-rich sports leagues in the world.
This project digs into 16 seasons of match and ball-by-ball data to answer real
cricket questions using Python data science tools.

---

## 📊 Analyses Covered

| # | Analysis | Technique Used |
|---|----------|----------------|
| 1 | Season-wise total runs & match count | Dual-axis bar + line chart |
| 2 | Top 10 batsmen by all-time runs | Horizontal bar, groupby sum |
| 3 | Top 10 bowlers by total wickets | Filtered dismissal types |
| 4 | Win percentage by team | value_counts, min-match filter |
| 5 | Toss decision impact on results | Boolean encoding, pie chart |
| 6 | Best venues by avg first-innings score | inning filter, groupby mean |
| 7 | Most Player of the Match awards | value_counts, annotated bar |
| ⭐ | Bonus: Correlation heatmap | df.corr(), sns.heatmap |

---

## 🚀 How to Run This Notebook

### Option 1 — Open Directly in Google Colab (Recommended)

1. Click the notebook file `IPL_Analysis_Colab.ipynb` above
2. Click **"Open in Colab"** button at the top of the file preview
3. Upload `matches.csv` and `deliveries.csv` using the 📂 Files panel (left sidebar in Colab)
4. Go to **Runtime → Run All**
5. All 7 charts will display inline and save as `.png` files

### Option 2 — Run Locally

```bash
pip install pandas numpy matplotlib seaborn
jupyter notebook IPL_Analysis_Colab.ipynb
```

---

## 📦 Dataset

| File | Description | Rows |
|------|-------------|------|
| `matches.csv` | One row per match — teams, winner, toss, venue | ~950 |
| `deliveries.csv` | One row per ball bowled — batsman, bowler, runs, wicket | ~179,000 |

**Source:** [IPL Complete Dataset 2008–2024 — Kaggle](https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020)

---

## 🛠️ Libraries Used

| Library | Purpose |
|---------|---------|
| `pandas` | Data loading, cleaning, groupby operations |
| `numpy` | Numerical calculations |
| `matplotlib` | Base plotting engine |
| `seaborn` | Statistical chart styling |

All libraries come **pre-installed** in Google Colab — no setup needed.

---

## 💡 Key Insights Found

- **Virat Kohli** is the all-time IPL run scorer across 15+ seasons with RCB
- **Lasith Malinga** leads wicket takers with his unorthodox slingy action
- **Mumbai Indians & CSK** have win rates above 55% — driven by captaincy stability
- Winning the toss leads to a win only **~50% of the time** — toss is overrated
- Modern teams choose to **field first 65–70%** of the time — chasing is the dominant strategy
- **Wankhede & Brabourne** (Mumbai) produce the highest first-innings averages

---

## 📁 Repository Structure
ipl-data-analysis/
│
├── IPL_Analysis_Colab.ipynb   ← Main analysis notebook
├── matches.csv                ← Match-level dataset
├── deliveries.csv             ← Ball-by-ball dataset
└── README.md                  

---

## 🔭 Future Work / Extensions

- [ ] Economy rate leaderboard (bowlers with 500+ balls)
- [ ] Powerplay vs death over scoring trends by season
- [ ] Head-to-head win/loss function for any two teams
- [ ] Strike rate leaders (batsmen with 500+ balls faced)
- [ ] Match winner predictor using scikit-learn

---
