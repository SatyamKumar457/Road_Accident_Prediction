# 🚗 Road Accident Severity Prediction  

> **A Machine Learning project to predict road accident severity using regression models**  
> _Developed for Kaggle Playground Series – Season 5, Episode 10_  

---

## 🧾 Project Metadata (YAML Overview)
```yaml
project:
  name: "Road Accident Severity Prediction"
  author: "Satyam Kumar"
  repository: "https://github.com/SatyamKumar457/Road_Accident_Prediction"
  license: "MIT"
  kaggle_competition: "https://www.kaggle.com/competitions/playground-series-s5e10"
  type: "Supervised Regression"
  target_variable: "Severity"
  language: "Python 3.11"
```

---

## 🎯 Overview  
This project focuses on **predicting road accident severity** using machine learning models trained on environmental, temporal, and road-related factors.  
By analyzing large-scale accident data, the goal is to uncover patterns and build predictive systems that assist in road safety analysis.

---

## 📊 Dataset Summary
```yaml
dataset:
  source: "Kaggle Playground Series S5E10"
  format: "CSV (train/test)"
  features:
    - 🌦️ Weather and visibility
    - 🛣️ Road surface and lighting
    - 🚗 Vehicle and accident characteristics
    - ⏱️ Temporal attributes (day, month, time)
  target: "Severity"
```

---

## ⚙️ Project Structure
```yaml
structure:
  data:
    - train.csv
    - test.csv
    - sample_submission.csv
  notebooks:
    - EDA.ipynb
    - Feature_Engineering.ipynb
    - Model_Training.ipynb
    - Final_Submission.ipynb
  models:
    - gradient_boosting.pkl
    - random_forest.pkl
    - xgboost.pkl
  submissions:
    - submission.csv
    - submission1.csv
    - submission2.csv
  files:
    - requirements.txt
    - LICENSE
    - README.md
```

---

## 🤖 Models and Evaluation  
| 🧠 Model | 📝 Description | 🎯 R² (Validation) | 🏆 Kaggle Score |
|-----------|----------------|--------------------|----------------|
| **📈 Linear Regression** | Baseline model | 0.82 | – |
| **🌲 Random Forest Regressor** | Tuned ensemble via GridSearchCV | 0.90 | 0.05581 |
| **🔥 Gradient Boosting Regressor** | Best-performing ensemble | **0.92** | **0.05579** |
| **⚡ XGBoost Regressor** | Regularized boosting model | 0.89 | 0.05582 |
| **🐈 CatBoost Regressor** | Handles categorical features | 0.91 | – |

> ✅ **Best Model:** Gradient Boosting Regressor  
> 🏁 **Leaderboard Score:** `0.05579`  
> 📌 Consistent across validation and public board.

---

## 🧠 Workflow  
```yaml
workflow:
  - Step 1: Data Cleaning → Handle nulls, encode categories, remove outliers.
  - Step 2: Exploratory Data Analysis → Visualize distributions, correlations.
  - Step 3: Feature Engineering → Time-based, weather, and interaction features.
  - Step 4: Model Training → Ensemble and gradient-based models.
  - Step 5: Evaluation → Metrics: R², RMSE, Kaggle leaderboard.
  - Step 6: Final Submission → Generate predictions and submit CSV.
```

---

## 📈 Results Summary
- 🏆 **Best Model:** Gradient Boosting Regressor  
- 📊 **Validation R²:** `0.92`  
- 💯 **Leaderboard Score:** `0.05579`  
- 🧩 **Rank:** Top consistent performer  
- 🔍 Improved generalization using **cross-validation** and **early stopping**  

---

## 🧰 Tech Stack
```yaml
technologies_used:
  - Python 🐍
  - Scikit-learn ⚙️
  - NumPy / Pandas 🧮
  - Matplotlib / Seaborn 📊
  - XGBoost ⚡
  - CatBoost 🐈
  - Kaggle API 🔌
```

---

## 💡 Future Enhancements
- 🧱 Implement model stacking and blending  
- 🧭 Add SHAP/LIME for feature interpretability  
- 🧠 Explore deep learning tabular models (TabNet, AutoGluon)  
- 📊 Build a Streamlit dashboard for interactive visualization  

---

## 👨‍💻 Author Info
```yaml
author:
  name: "Satyam Kumar"
  github: "https://github.com/SatyamKumar457"
  kaggle: "https://www.kaggle.com/"
  interests: ["AI", "Data Science", "Machine Learning"]
  note: "Exploring ML models that solve real-world safety problems."
```

---

## 📜 License
This project is licensed under the **MIT License** — you are free to use, modify, and distribute with attribution.  

---

## 🧩 Example Visualization
> *(Optional — you can add your leaderboard screenshot or R² comparison bar plot here)*  

```yaml
visualizations:
  - file: "figures/model_r2_comparison.png"
    description: "R² score comparison for all trained models."
```
