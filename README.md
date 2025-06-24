# player-behavior-analytics

# 🎮 Player Behavior Analysis & Churn Prediction in Online Multiplayer Game

This project explores simulated gameplay data to analyze player behavior, uncover key engagement patterns, and build predictive models to identify potential churn. Inspired by the types of analytics used in the gaming industry, especially at companies like Rockstar Games, the project demonstrates how data-driven insights can help enhance player retention and gameplay experience.

## 📊 Project Overview

- **Dataset:** Synthetic dataset simulating ~10,000 multiplayer player sessions
- **Tech Stack:** Python, Pandas, NumPy, Seaborn, Scikit-learn, Matplotlib, SQL
- **Goal:** Understand behavioral clusters and predict player churn using machine learning

## 🧠 Key Objectives

- Analyze in-game event logs to extract behavior patterns
- Cluster players based on session frequency, playstyle, and achievements
- Predict potential churners using classification models
- Visualize insights to drive game design and retention strategies

## 🔍 Exploratory Data Analysis (EDA)

- Analyzed features such as `session_count`, `average_session_length`, `level_retries`, `achievement_unlocks`, `in-game purchases`, and `last_login`.
- Discovered engagement drop-off around specific game levels.
- Identified peak activity hours and platform-specific trends (PC vs Console).

## 🤖 Machine Learning Models

- **Clustering:** Used K-Means and DBSCAN to segment players into behavioral cohorts (e.g., “Hardcore”, “Casual”, “At-Risk”).  
- **Classification Models:** 
  - Logistic Regression
  - Random Forest
  - XGBoost  
- **Performance:** Achieved up to **85% accuracy** in predicting churn risk. Tuned models with cross-validation and grid search.

## 📈 Visualizations

- Session heatmaps  
- Engagement funnels  
- Churn risk distributions  
- Cluster visualizations using PCA/t-SNE

## 📌 Results & Recommendations

- Identified ~18% of players with high churn probability based on recent inactivity, low achievements, and repeated failures.  
- Suggested in-game incentives (bonus levels, in-game currency) to re-engage at-risk players.  
- Recommended dynamic difficulty adjustment for frustration-prone segments.

## 💡 Takeaways

- Player behavioral data provides immense value in improving retention and satisfaction.
- Clustering and churn prediction can inform personalized game experiences.
- Strong alignment with data science roles in the gaming industry, such as at Rockstar Games.

## 🔧 Future Work

- Integrate time-series analysis for session progression trends  
- Deploy a real-time churn detection dashboard using Streamlit or Power BI  
- Incorporate NLP to analyze player chat/emotion sentiment


