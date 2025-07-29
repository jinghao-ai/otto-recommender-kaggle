# OTTO Recommender System – Days 1 to 21

This repository documents a self-directed Kaggle project exploring the OTTO Recommender System dataset.

## ✅ Completed Days

### Day 1 – Data Loading
- Loaded and explored OTTO's raw Parquet dataset.
- Mapped numeric event types to human-readable labels.

### Day 2 – Behavior Analysis
- Analyzed the distribution of clicks, carts, and orders.
- Visualized behavior counts and session length distributions.

### Day 3 – Conversion Funnel
- Built a pivot table to summarize session-level behavior.
- Created boolean flags and visualized the user behavior funnel.

### Day 4 – Sequential Pattern Mining
- Constructed user action sequences ordered by timestamp.
- Extracted frequent behavior paths and plotted common sequences.

### Day 5 – Item-Level Popularity Features
- Calculated total clicks, carts, and orders for each item.
- Created click-to-cart rate (CTR) and click-to-order rate (CVR).
- Visualized top 20 most clicked items.
- Saved all item-level stats for future model use.

## 📂 Structure

- `notebook/`: Contains Day 1–4 Jupyter Notebooks.
- `visualizations/`: Visual output from matplotlib charts.
- `README.md`: Project overview and progress.

## 📌 Author

Prepared by Zhang JingHao for application to NTU Singapore.
