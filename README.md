# 🎯 Fitness App Marketing Analytics

## 📌 Overview
This project optimizes marketing for a subscription-based fitness app by:
- Building a lead scoring model to predict conversions (AUC: 0.86).
- Segmenting customers for targeted campaigns.
- Optimizing ad spend to reduce customer acquisition cost (CAC) by ~21%.
- Using geospatial and socioeconomic data to identify high-value audiences.

## 🧠 Hypothesis
High-income, urban users aged 25–40 with high engagement are more likely to convert, and reallocating ad spend to target them reduces CAC.

## 📊 Data
- **users.csv**: User demographics, behavior, and conversion status.
- **ads.csv**: Ad campaign performance (spend, impressions, clicks, conversions).
- **zip_income.csv**: Socioeconomic data by ZIP code (income, education, urban/rural).

## ⚙️ Methods
- **EDA**: Conversion rates by age, gender, device, income, and urban classification.
- **Feature Engineering**: Engagement score, one-hot encoding, socioeconomic features.
- **Lead Scoring**: Random Forest classifier (AUC: 0.86).
- **Segmentation**: K-Means clustering (4 segments).
- **Ad Optimization**: Simulated budget reallocation to top-performing channels.

## 📈 Key Results
- **Lead Scoring**: AUC of 0.86, with engagement_score and median_income as top features.
- **Segmentation**: Identified high-value segment (urban, 25–35, high-income, high-engagement).
- **Ad Optimization**: Reallocating 20% of budget to Instagram reduced CAC by ~21%.
- **Geospatial Insights**: Urban areas show higher conversion density.

## 📎 Files
- `notebook.ipynb`: Full analysis code.
- `app.py`: Streamlit dashboard code.
- `*.png`: Visualization outputs.
- `conversion_heatmap.html`: Geospatial heatmap.
- `*.csv`: Processed datasets and model outputs.
- `lead_scoring_model.pkl`: Trained Random Forest model.

## 🛠️ Setup
1. Clone the repo: `git clone [your-repo-url]`
2. Install dependencies: `pip install -r requirements.txt`
3. Run notebook: `jupyter notebook notebook.ipynb`
4. Run dashboard: `streamlit run app.py`

## 📸 Visuals
![Conversion by Age](age_conversion.png)
![Feature Importance](feature_importance.png)
![Customer Segments](customer_segments.png)

## 🧩 Future Work
- Real-time ad bidding model.
- Lifetime value (LTV) prediction.
- Integration with live ad platform APIs.

## 📬 Contact
Built by [Mohammadreza soltani].
