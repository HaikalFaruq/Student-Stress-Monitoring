# 🎓 Student Stress Monitoring Project
> *"Understanding stress today, shaping healthier students tomorrow."*

---

## 📖 Project Overview
Student stress is a growing concern in modern education, driven by academic pressure, lifestyle habits, and mental health challenges. High stress levels not only affect academic performance but also impact long-term well-being.  

This project aims to **analyze student stress levels through psychological, lifestyle, and academic factors** to identify the strongest predictors and provide actionable solutions for prevention and support.  

The core problem addressed is that many universities lack a **data-driven understanding** of what truly influences student stress, making interventions reactive rather than proactive.  

Our approach includes:  
1. **Data Preprocessing** – handling duplicates, scaling, encoding, and outliers.  
2. **Exploratory Data Analysis** – studying distributions, correlations, and feature importance.  
3. **Modeling & Dimensionality Reduction** – applying PCA, mutual information scores, and ensemble methods.  
4. **Actionable Insights** – transforming results into practical recommendations such as counseling, academic mentoring, and lifestyle improvement.  

Through this structured process, the project delivers **evidence-based insights** that empower institutions to build healthier and more supportive learning environments.

---

## 🔬 Analysis Process

| Step | Method & Technique | Reason for Use |
|------|-------------------|----------------|
| **1. Data Understanding** | Checked records, features, duplicates, and missing values | Ensures data quality before analysis |
| **2. Preprocessing** | Scaling (StandardScaler/MinMaxScaler), encoding categorical vars, handling outliers/duplicates | Creates clean, balanced input for models |
| **3. EDA (Exploratory Data Analysis)** | Visualizations (distribution plots, heatmaps, correlations) | Identifies patterns and feature relationships |
| **4. Feature Selection** | Correlation analysis & mutual information scores | Focus on strongest predictors (e.g., anxiety, depression, sleep quality) |
| **5. Dimensionality Reduction** | Principal Component Analysis (PCA) | Reduces complexity, avoids overfitting |
| **6. Modeling** | Ensemble methods (Random Forest, XGBoost) | Robust against noise & multicollinearity |
| **7. Insights & Recommendations** | Translate results into mental health, academic, and lifestyle strategies | Ensures findings are actionable for institutions |


---

## 📂 Raw Dataset
- Source: [Kaggle – Student Stress Monitoring Datasets](https://www.kaggle.com/datasets/mdsultanulislamovi/student-stress-monitoring-datasets)  
- Files included:
  - `StressLevelDataset.csv` → structured numeric dataset  
  - `Stress_Dataset.csv` → survey-based dataset with detailed stress factors  

---

## 📊 Visualizations

| Visualization | Preview | Explanation |
|---------------|---------|-------------|
| **Stress Level Distribution** | <img width="2531" height="1630" alt="stress_level_distribution" src="https://github.com/user-attachments/assets/db7c9663-25bd-407f-9427-681b90e7fbce" /> | Shows how stress is divided among students (low, medium, high). Distribution is fairly balanced, with a slightly higher count of low and high stress compared to medium. |
| **Types of Stress Experienced** | <img width="3541" height="1768" alt="stress_types_distribution" src="https://github.com/user-attachments/assets/58e84bb9-c935-4434-a91d-74af4d3bba70" /> | Most students reported **Eustress (positive stress)** which motivates performance, while fewer experienced distress or no stress. |
| **Outlier Percentages by Feature** | <img width="4171" height="2370" alt="outlier_percentages" src="https://github.com/user-attachments/assets/8a8d9ca7-9130-4865-b09b-4eb082d5f705" /> | Highlights which features contain significant outliers. **Age** and **emotional factors** show the highest percentage of anomalies. |
| **Correlation Matrix** | <img width="5505" height="5157" alt="correlation_matrix" src="https://github.com/user-attachments/assets/d5f9891d-3d29-4c28-b2fb-3f43e3b93891" /> | Displays feature-to-feature relationships. Stronger correlations appear in lifestyle and psychological features. |
| **Feature Distributions** | <img width="5967" height="10764" alt="feature_distributions" src="https://github.com/user-attachments/assets/eabfd154-1bf7-4f62-b195-66fce8d7f028" /> | Shows frequency distributions for all features. Most variables are normally distributed but skewed toward mid-levels (2–3 on Likert scales). |
| **Mutual Information Scores** | <img width="2966" height="3572" alt="mutual_information_scores" src="https://github.com/user-attachments/assets/d2100598-fdb2-4ad6-bafd-52d02acd72bd" /> | Identifies the most important predictors of stress. **Heartbeat/Palpitations** and **Anxiety** are the top factors. |
| **PCA Analysis** | <img width="4767" height="1772" alt="pca_analysis" src="https://github.com/user-attachments/assets/65b27bf1-3607-4b48-9ede-2d87a33d82f7" /> | Principal Component Analysis shows that ~15 components explain ~95% of dataset variance. Useful for dimensionality reduction. |
| **Correlations with Stress Experience** | <img width="2965" height="3572" alt="stress_correlations" src="https://github.com/user-attachments/assets/ad7efd88-08d8-4e7a-aa6e-c61bf421902d" /> | Strongest correlations with stress experience: **Heartbeat issues, Anxiety, Academic pressure, and Sleep problems**. |
  | **Stress Experience Distribution** | <img width="2531" height="1630" alt="stress_experience_distribution" src="https://github.com/user-attachments/assets/7ffc5711-d65f-4993-a23d-d4933ddff052" /> | Most students fall into **moderate stress experience levels (2–3)**, with fewer at extreme levels (1 and 5). |

---

## 🔎 Insights & Findings
✅ **Anxiety & Depression** → strongest predictors of stress.  
✅ **Sleep Quality** → poor sleep strongly increases stress.  
✅ **Academic Pressure** → low performance + heavy study load = higher stress.  
✅ **Self-Esteem** → acts as a protective shield against stress.  

---


## 💡 Recommendations (Preprocessing & Modeling)

| Dataset | Preprocessing Recommendations |
|---------|--------------------------------|
| **STRESS SURVEY DATASET** (843 records, 26 features) | - Apply **scaling** (StandardScaler/MinMaxScaler)<br>- Start with **top 1 feature(s)** for feature selection<br>- Encode categorical variable (stress type) using **one-hot encoding**<br>- Use **ensemble methods** (e.g., Random Forest, XGBoost) for robustness<br>- Fix **duplicate column name issue** |
| **STRESS LEVEL DATASET** (1100 records, 21 features) | - Apply **scaling** (StandardScaler/MinMaxScaler)<br>- Start with **top 20 features** for feature selection<br>- Handle **multicollinearity** between features if detected<br>- Use **ensemble methods** (e.g., Random Forest, XGBoost) for robust predictions |

---

## 📝 Conclusion

| Key Insight | Concrete Action | Real Impact |
|-------------|-----------------|-------------|
| **Anxiety & depression are strongest predictors of stress** | Provide regular counseling and mental health programs | Reduces psychological burden and builds resilience |
| **Poor sleep quality worsens stress** | Launch campus-wide sleep & lifestyle awareness campaigns | Improves overall student health and productivity |
| **Academic & career pressures drive stress** | Offer mentorship and career guidance services | Enhances academic performance and career readiness |
| **Bullying and weak social support increase stress** | Enforce anti-bullying policies & strengthen peer support groups | Creates safer and more supportive campus environment |
| **Physical health issues (blood pressure, headaches)** | Routine health checkups and wellness programs | Detects early risks and prevents long-term health problems |

---

## 🤖 AI Support Explanation
We applied AI & analytics to:
- 📊 Preprocess and clean raw dataset  
- 📈 Perform **EDA & correlation analysis**  
- 🔍 Identify **key stress predictors**  
- 📝 Generate **data-driven recommendations**  

This ensures insights are **evidence-based** and **actionable**.

---

## 🏆 Why This Project Matters
Stress is a silent epidemic among students. By analyzing real-world data, this project empowers:  
- 🎓 Universities → to design better support systems  
- 👩‍🎓 Students → to understand & manage their stress  
- 🧑‍💻 Researchers → to explore mental health analytics with AI  

---

## ✨ Final Note
*"Healthy minds build a brighter future."*  
This project is not just about **numbers**, but about **lives**.  
Together, let’s make learning a little less stressful 💙
