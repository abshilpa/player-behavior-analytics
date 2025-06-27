# 🎮 Player Behavior Analysis & Engagement Prediction

This project explores player behavior using a synthetic dataset simulating a real-world gaming environment. We analyze player engagement patterns, segment player types using clustering, and build predictive models to forecast engagement levels (High, Medium, Low). 

The work demonstrates the use of machine learning in gaming analytics, aligning with data science practices at companies like **  gaming Industry **.

---

## 📌 Project Objectives

- Explore patterns in player activity and in-game behavior through **exploratory data analysis (EDA)**.
- Segment players based on behavioral attributes using **unsupervised learning (K-Means + PCA)**.
- Build and compare supervised models to predict player **EngagementLevel** (High, Medium, Low).
- Tune multiple algorithms (Random Forest, XGBoost, CatBoost) for optimal performance.
- Identify key features influencing engagement to inform game design and retention strategies.

---

## 📊 Dataset Overview

- **Source:** Kaggle – [Predict Online Gaming Behavior](https://www.kaggle.com/datasets/rabielkharoua/predict-online-gaming-behavior)
- **Type:** Synthetic dataset (educational use)
- **Size:** 40,034 player records
- **Target Variable:** `EngagementLevel` (0 = High, 1 = Medium, 2 = Low)
- **Key Features:**  
  `SessionsPerWeek`, `PlayTimeHours`, `AvgSessionDurationMinutes`,  
  `PlayerLevel`, `AchievementsUnlocked`, `InGamePurchases`, `GameGenre`, etc.

---

## 🔍 Exploratory Data Analysis (EDA)

- The dataset shows class imbalance with more players in the “Low Engagement” group.
- Strong patterns observed between engagement level and features like session frequency, duration, and achievements.
- All categorical features were label-encoded to prepare for modeling.

---

## 🧠 Clustering & Player Segmentation

- Applied **K-Means (k=3)** to group players into behavioral segments:
  - **Cluster 0:** Casual Players  
  - **Cluster 1:** Completionists  
  - **Cluster 2:** Consistent Engagers  
- Used **PCA** to reduce dimensions and visualize clusters effectively.

---

## 🤖 Supervised Modeling: Engagement Prediction

Trained and tuned multiple classifiers to predict player engagement:

| Model                 | Accuracy | Precision | Recall | F1-Score |
|-----------------------|----------|-----------|--------|----------|
| Random Forest (Tuned)  | 91.06%   | 0.91      | 0.90   | 0.91     |
| XGBoost (Tuned)        | 91.56%   | 0.92      | 0.91   | 0.91     |
| CatBoost (Default)     | 91.39%   | 0.91      | 0.90   | 0.91     |
| **CatBoost (Tuned)**   | **91.77%** | **0.92**  | **0.91** | **0.91** |

- **Top Predictors:** `SessionsPerWeek`, `AvgSessionDurationMinutes`, `AchievementsUnlocked`, `PlayerLevel`

---

## 🌟 Key Findings

- Players with higher session frequency and longer session durations tend to have higher engagement.
- Cluster analysis revealed meaningful segments, supporting targeted retention strategies.
- **CatBoost (Tuned)** delivered the best overall accuracy with minimal tuning effort, ideal for deployment in gaming analytics.

---

## 🛠 Tools & Libraries

- **Languages & Frameworks:** Python, Jupyter Notebooks
- **Libraries:** Pandas, NumPy, Scikit-learn, XGBoost, CatBoost, Seaborn, Matplotlib

---

## 🚀 Why This Project Matters

This project showcases how data science and machine learning can be applied to gaming data to:
- Enhance player experience
- Inform design decisions
- Improve retention and engagement

It reflects the type of analytics work that supports to build data-powered entertainment experiences.



