# Social Media Marketing Analytics & Engagement Prediction

An end-to-end data analysis project: cleaning, exploratory data analysis (EDA), and a
machine learning model that predicts social media post **engagement rate** from
features known *before* publishing (platform, post type, timing, hashtags, ad spend, etc.).

## Files
- `social_media_engagement_analysis.ipynb` — main notebook (EDA + ML model, fully executed with outputs/plots)
- `social_media_marketing.csv` — dataset (2,500 posts, synthetic but realistic; easy to swap for real API/Kaggle data)

## What it covers
1. Data cleaning (missing values, duplicates)
2. EDA — engagement by platform, post type, best posting time (day×hour heatmap), hashtag effect, paid vs. organic, correlation heatmap
3. Feature engineering + a `RandomForestRegressor` model to predict engagement rate
4. Model evaluation (MAE, RMSE, R²) and feature importance analysis
5. Business insights + suggestions to extend the project with real data / NLP / deployment

## How to run
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook social_media_engagement_analysis.ipynb
```

## Resume bullet points (pick 1-2)
- Built an end-to-end social media analytics pipeline in Python (Pandas, Seaborn, Scikit-learn), analyzing 2,500+ posts across 5 platforms to identify engagement drivers.
- Engineered features and trained a Random Forest model to predict post engagement rate, achieving strong R² on held-out data, enabling data-driven content scheduling recommendations.
- Uncovered actionable marketing insights (best posting times, top-performing formats, hashtag saturation point) through exploratory data analysis and visualization.

## Possible extensions
- Replace synthetic data with a real dataset pulled from a platform API or Kaggle.
- Add NLP-based caption features (sentiment, emoji/keyword extraction).
- Compare against XGBoost/LightGBM.
- Wrap the model in a small Streamlit app for interactive "what engagement will my post get" predictions.
