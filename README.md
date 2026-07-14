# 📊 Social Media Marketing Analytics & Engagement Prediction

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML%20Model-F7931E)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

An end-to-end data analysis project that explores what drives engagement on social
media, and builds a machine learning model that **predicts a post's engagement rate
before it's even published** — using only features known in advance (platform, post
type, timing, hashtags, ad spend, etc.).

---

## 🎯 Problem Statement

Marketing teams post constantly but rarely know in advance which posts will perform
well. This project analyzes 2,500 posts across 5 platforms to answer:

- Which platform and post format drive the most engagement?
- When is the best time to post (day + hour)?
- Do hashtags and paid promotion actually help — and by how much?
- Can we predict a post's engagement rate before publishing it?

---

## 🗂️ Repository Structure

```
├── social_media_engagement_analysis.ipynb   # Main notebook — EDA + ML model (fully executed)
├── social_media_marketing.csv               # Dataset — 2,500 posts across 5 platforms
├── requirements.txt                         # Python dependencies
└── README.md
```

---

## 🔍 Key Findings

| Insight | Detail |
|---|---|
| **Best platform** | TikTok leads with median engagement of **2.79%**, followed by Instagram (2.35%) |
| **Best format** | Short-form video (Reels/Shorts) outperforms static images and text posts |
| **Best posting time** | Lunch (12–1 PM) and evening (6–9 PM) windows consistently show higher engagement |
| **Hashtags** | Engagement rises with hashtag count up to ~8–10 tags, then plateaus |
| **Paid vs organic** | Paid posts show higher median engagement (1.99% vs 1.70%) but with diminishing returns on spend |

*(Full charts and breakdowns are in the notebook.)*

---

## 🤖 Machine Learning Model

A `RandomForestRegressor` was trained to predict `engagement_rate_pct` from
pre-publish features (platform, post type, day/hour, hashtag count, caption length,
followers, ad spend, video duration).

| Metric | Score |
|---|---|
| **R²** | 0.645 |
| **MAE** | 0.41 percentage points |
| **RMSE** | 0.55 percentage points |

The model explains ~65% of the variance in engagement rate using only information
available *before* a post goes live — meaning a marketing team could test different
post plans and pick the one predicted to perform best.

---

## 🛠️ How to Run

```bash
git clone https://github.com/YOUR-USERNAME/social-media-engagement-prediction.git
cd social-media-engagement-prediction
pip install -r requirements.txt
jupyter notebook social_media_engagement_analysis.ipynb
```

---

## 📌 Tech Stack

`Python` · `Pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `Scikit-learn` · `Jupyter`

---

## 🚀 Possible Extensions

- Swap the synthetic dataset for real data pulled via a platform API or Kaggle.
- Add NLP features from actual caption text (sentiment, emoji/keyword extraction).
- Compare against XGBoost/LightGBM for better accuracy.
- Deploy the model in a Streamlit app for live "predict my post's engagement" demos.

---

## 👤 Author

*Add your name, LinkedIn, and portfolio link here.*
