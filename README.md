<h1 align="center">🍷💖 Wine Quality Classifier (Binary ML Project)</h1>
<p align="center">
  <i>Created by <b>Tenika Powell</b> | Data Science & Machine Learning Student</i>  
</p>

---

## 💡 Project Overview
This project uses **machine learning** to predict whether a red wine is **Good (1)** or **Not Good (0)** based on its chemical composition.  
The original dataset rated wines from 3–8, but it was reframed into a **binary classification problem** for better accuracy and clarity.

---

## 🧠 Objective
**Goal:** Teach an AI model to identify high-quality wines using chemical features like:
- Fixed & volatile acidity  
- Residual sugar & sulphates  
- Alcohol content  
- Density & pH  

---

## ⚙️ Tools & Libraries
| Category | Libraries Used |
|-----------|----------------|
| Data Handling | Pandas, NumPy |
| Machine Learning | Scikit-Learn, XGBoost |
| Balancing | imbalanced-learn (SMOTE) |
| Visualization | Matplotlib, Seaborn |
| Optimization | GridSearchCV, Cross-Validation |

---

## 🧩 Workflow Summary
1. **Data Loading:** UCI Red Wine Quality dataset.  
2. **Label Creation:** Converted “quality” scores into:
   - `0` → Not Good (rating < 7)  
   - `1` → Good (rating ≥ 7)
3. **Feature Engineering:** Added new ratio & interaction features:
   - `acidity_ratio = fixed acidity / volatile acidity`  
   - `alcohol_density_ratio = alcohol / density`  
   - `sugar_sulphate_ratio = residual sugar / sulphates`  
   - `ph_alcohol_interact = pH * alcohol`
4. **Scaling:** Standardized all numeric features.  
5. **Balancing:** Used **SMOTE** to handle class imbalance.  
6. **Model Training:**  
   - **K-Nearest Neighbors (KNN)**  
   - **XGBoost (Gradient Boosting)**  
7. **Tuning:** GridSearchCV + 5-fold Cross-Validation.  
8. **Evaluation:** Accuracy, ROC–AUC, Precision–Recall, and confusion matrices.

---

## 📊 Model Results

| Model | Test Accuracy | ROC–AUC | PR–AUC | Notes |
|--------|----------------|----------|---------|-------|
| 🎯 **KNN** | **0.79 (79%)** | 0.82 | 0.80 | Performs well after SMOTE and scaling |
| ⚡ **XGBoost** | **0.85–0.87 (85–87%)** | **0.90+ ✅** | **0.86+ ✅** | Best model overall |

**Final Decision:**  
XGBoost achieved the **highest accuracy and generalization**, correctly identifying most “good” wines with minimal false positives.

---

## 🔍 Key Insights
- **Alcohol** and **sulphates** were the top predictors of wine quality.  
- The **alcohol-to-density ratio** was the strongest new feature.  
- Binary classification simplified the problem and boosted accuracy by **10–15%**.  
- Balancing data with SMOTE prevented bias toward lower-quality wines.  

---

## 💖 ROC–AUC & Precision–Recall Performance
- Both curves show **strong separability** between good and not-good wines.  
- XGBoost maintained higher precision and recall, confirming robustness.  
- AUC ≈ **0.90+**, which means the model ranks good wines correctly 9/10 times.

---

## 🧠 Lessons Learned
- **Feature scaling and balancing** are critical for fair ML comparisons.  
- **Feature engineering** can unlock patterns not obvious in raw data.  
- Always verify results using **multiple metrics**, not just accuracy.

---

## 🌷 Final Summary
| Metric | KNN | XGBoost |
|---------|-----|----------|
| Accuracy | 79% | **85–87% ✅** |
| ROC–AUC | 0.82 | **0.90+ ✅** |
| PR–AUC | 0.80 | **0.86+ ✅** |

💎 **Conclusion:**  
> Reframing the problem into binary classification, balancing the data, and tuning advanced models allowed me to achieve over **85% accuracy**.  
> XGBoost proved to be the most powerful and reliable model for predicting wine quality.

---

## 🚀 GitHub Project
**Repository:** [Nikkilabesf/k-nearest-neighbors-project-tutorial](https://github.com/Nikkilabesf/k-nearest-neighbors-project-tutorial)  
**Created with:** 💖, ☕, and Python  
**By:** *Tenika Powell*

---

