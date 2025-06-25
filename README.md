# player-behavior-analytics

# 🎮 Player Behavior Analysis & Engagement Prediction

This project explores online player behavior using a synthetic dataset that simulates real-world gaming environments. We analyze player engagement, uncover behavioral segments using clustering, and build predictive models to forecast engagement levels. 

## 📌 Overview

- 🔍 Behavioral segmentation of players using **K-Means clustering**
- 🧠 Predictive modeling of player **EngagementLevel** (High, Medium, Low)
- 📊 Feature importance analysis to guide game design and retention strategies
- 💻 Tools: Python, Pandas, Seaborn, Scikit-learn, PCA, Random Forest

---

## 📂 Dataset

**Source:** [Kaggle - Predict Online Gaming Behavior](https://www.kaggle.com/datasets)  
**Size:** 40,034 rows × 13 columns  
**Key Features:**

- `PlayTimeHours`, `SessionsPerWeek`, `AvgSessionDurationMinutes`
- `AchievementsUnlocked`, `GameDifficulty`, `InGamePurchases`
- `EngagementLevel` (Target): High, Medium, Low

---

## 📊 Exploratory Data Analysis (EDA)

- Distribution of engagement levels shows class imbalance skewed toward “Low” engagement
- Key patterns discovered between session frequency, duration, and achievement unlocking
- Categorical features like `Gender`, `GameGenre`, and `Location` were label-encoded

---

## 🔍 Clustering Player Types

- Applied **K-Means** with `n_clusters=3`
- Used **PCA** to reduce feature space for 2D visualization
- Identified three player segments:
  - **Cluster 0:** Casual Players  
  - **Cluster 1:** Completionists  
  - **Cluster 2:** Consistent Engagers

---

## 🤖 Engagement Prediction (Supervised Learning)

### Model: Random Forest Classifier

- **Accuracy:** `91%`
- **Classification Report:**
  - F1-score: High (0.90), Medium (0.89), Low (0.93)
- **Feature Importance:**
  - Top predictors: `SessionsPerWeek`, `AvgSessionDurationMinutes`, `PlayTimeHours`

---

## 🧠 Key Takeaways

- High session frequency and longer session durations strongly correlate with higher engagement.
- Machine learning models can effectively predict player behavior and inform in-game design.
- Cluster analysis provides valuable segmentation for targeted retention strategies.

---

## 🛠️ Tools & Technologies

- Python, Pandas, NumPy, Seaborn, Matplotlib
- Scikit-learn (Random Forest, KMeans, PCA, LabelEncoder, StandardScaler)
- Jupyter Notebooks



