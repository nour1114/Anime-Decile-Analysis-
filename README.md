# 📊 Anime Decile Analysis (MyAnimeList Dataset)

This project performs **decile-based segmentation analysis** on anime popularity using the MyAnimeList dataset.

## 🎯 Objective
Divide anime into 10 equal-frequency groups based on popularity (Members) and analyze:
- Mean Score per group
- Total Members per group
- Cumulative contribution of popularity

## 🧠 Key Concepts
- Pandas `pd.qcut` for quantile-based binning
- GroupBy aggregation
- Cumulative distribution analysis
- Data segmentation (deciles)

## 📦 Output
A DataFrame indexed by deciles (01–10) with:

| Column | Description |
|--------|------------|
| MeanScore | Average rating per decile |
| TotalMembers | Total audience size |
| CumulativePct | % contribution to total popularity |

## 🚀 How to Run

```bash
pip install -r requirements.txt
python src/decile_analysis.py
📊 Insight

Higher deciles contain fewer anime but disproportionately higher audience engagement — a classic long-tail distribution pattern.

📁 Dataset Source

MyAnimeList Dataset: https://github.com/Hernan4444/MyAnimeList-Database


---

# 📦 requirements.txt


pandas
numpy
matplotlib
