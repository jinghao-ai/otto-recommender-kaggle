# OTTO Recommender System – Days 1 to 20

This repository documents a self-directed Kaggle project exploring the OTTO Recommender System dataset.

## 🛒 OTTO Recommender System (Kaggle Project)

This repository documents my learning journey through the OTTO RecSys Kaggle competition.  
The project is structured in daily progress notebooks, each extracting and engineering features from clickstream data.

✅ Purpose: Strengthen my data science foundations  


Notebook highlights:
- Data loading & EDA
- Behavior statistics & funnels
- Sequential pattern mining
- Item-level popularity features

## ✅ Completed Days

# Day 1 - Data Loading

**Goal:** Load and inspect the raw interaction data from the OTTO recommender system dataset.

## Tasks
- Load `train.parquet` using `pandas`
- Display sample rows and check for column names, data types, and null values
- Understand the meaning of each column (`session`, `aid`, `ts`, `type`)

## Key Concepts
- DataFrame operations with `pandas`
- Basic I/O operations and dataset inspection


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

### Day 6 – Session-Level User Features
- Calculated the number of clicks, carts, and orders per session.
- Computed click ratio and session length for each user.
- Extracted active time period features (min, max, avg hour).
- Saved all session-level features for future training steps.

## 📘 Day 7 – Candidate Generation: Popularity-Based Recall

### ✅ Goal
This notebook implements a simple candidate recall method based on item popularity.
I use the most popular items (based on clicks, carts, and orders) and assign them to each session as candidate items.

### 🔍 Steps

1. Load original session event data
2. Map action types to human-readable strings
3. Aggregate item popularity by action type
4. Construct candidate session × item pairs
5. Save results for future modeling

### 🧠 Knowledge Points

- Data aggregation using `groupby` and `size`
- Using `np.repeat` and `np.tile` to generate matrix-style candidate data
- Understanding two-stage recommendation systems

## 📂 Structure

- `notebook/`: Contains Day 1–20 Jupyter Notebooks.
- `visualizations/`: Visual output from matplotlib charts.
- `README.md`: Project overview and progress.

## 📌 Author

Prepared by Zhang JingHao 
🎯 Goal: Prepare for research and scholarship application at NTU Singapore
