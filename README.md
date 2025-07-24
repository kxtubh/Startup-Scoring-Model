# Startup Scoring Model

A comprehensive scoring system that evaluates startup health and success potential using two distinct approaches: **Weighted Scoring** and **Unsupervised Machine Learning**.

## 🎯 Overview

This project analyzes startup performance across multiple dimensions to generate health scores from 0-100, helping investors and stakeholders make data-driven decisions.

## 📊 Dataset Features

- `team_experience` - Experience level of founding team
- `market_size_million_usd` - Total addressable market size
- `monthly_active_users` - User traction metrics
- `monthly_burn_rate_inr` - Monthly cash burn rate
- `funds_raised_inr` - Total funding raised
- `valuation_inr` - Current company valuation

## 🔧 Two Scoring Approaches

### 1. **Weighted Scoring Method** (Primary)
A rule-based approach using expert-defined weights:
- **Team Experience**: 20% - Founding team quality
- **Monthly Active Users**: 25% - Traction (highest weight)
- **Market Size**: 15% - Market opportunity
- **Burn Rate**: 15% - Financial efficiency (inverted)
- **Funds Raised**: 15% - Funding validation
- **Valuation**: 10% - Current market value

### 2. **Unsupervised Learning Method** (Alternative)
- **K-Means Clustering**: Segments startups into 4 distinct groups
- **Pattern Recognition**: Identifies natural groupings in startup characteristics
- **Interactive Visualization**: Plotly-based scatter plots for exploration


## 📈 Key Features

- **Data Preprocessing**: Min-Max normalization for fair comparison
- **Burn Rate Inversion**: Lower burn rates receive higher scores
- **Comprehensive Ranking**: Top/bottom 10 startup identification
- **Visual Analytics**: Distribution plots, correlation heatmaps, and interactive charts
- **Detailed Analysis**: Explains why top/bottom performers scored as they did

## 📊 Outputs

1. **Health Scores**: 0-100 scale for all startups
2. **Rankings**: Sorted list from best to worst performing
3. **Visualizations**: 
   - Score distribution histogram
   - Top 20 performance bar chart
   - Feature correlation matrix
   - Interactive scatter plots with clustering
4. **Insights**: Detailed breakdown of top and bottom performers

## 🔍 Key Insights

The model reveals that **user traction** (25% weight) is the most critical factor, followed by team experience and market dynamics. Financial metrics like burn rate and funding provide important context but are weighted lower.

## 📋 Requirements

```
pandas
numpy
matplotlib
seaborn
scikit-learn
plotly
```

## 📁 Files

- `startup_scoring.py` - Main scoring algorithm
- `Startup_Scoring_Dataset.csv` - Input dataset (required)

## 🤝 Usage

1. Ensure `Startup_Scoring_Dataset.csv` is in the same directory
2. Run the script to generate scores and visualizations
3. Review top/bottom performers and clustering results
4. Use interactive plots for deeper analysis

---

*A data-driven approach to startup evaluation combining domain expertise with machine learning insights.*
