<h1 align="center">💖🍷 Wine Quality Classifier – KNN Model 💻✨</h1>

<p align="center">
  <i>A stylish machine learning project blending data, elegance, and science.</i><br>
  <b>Created by: Tenika Powell</b> 🌸
</p>

---

## 💡 Project Overview
This project uses **K-Nearest Neighbors (KNN)** to predict the quality of red wine based on its chemical makeup.  
Each wine sample includes properties like acidity, sugar, pH, and alcohol level — all used to determine if a wine is **Low**, **Medium**, or **High quality**.  

👩🏽‍🔬 Think of it as your AI-powered sommelier — picking the best bottle using pure data.

---

## 🧠 Machine Learning Pipeline
💻 **Steps used:**
1. ✨ Load dataset from the UCI Wine Quality Repository  
2. 🍇 Convert the numeric `quality` into labeled categories (`0`, `1`, `2`)  
3. 🧼 Scale the data using `StandardScaler`  
4. 💖 Train a **KNN model**  
5. 🎯 Optimize with `GridSearchCV` (tested multiple `k`, `weights`, and `metrics`)  
6. 💫 Evaluate with accuracy, confusion matrix, and classification report  
7. 🌈 Combine with an **Ensemble (VotingClassifier)** for an extra accuracy boost  

---

## 💻 Tech Stack
| 🧩 Category | ⚙️ Tools |
|--------------|----------|
| Language | Python |
| Data Handling | Pandas, NumPy |
| ML Framework | Scikit-Learn |
| Visualization | Matplotlib, Seaborn |
| Optimization | GridSearchCV, VotingClassifier |

---

## 📊 Model Results
| 🧠 Model | ✨ Description | 🎯 Accuracy |
|-----------|----------------|-------------|
| KNN (Default) | k=5 | ~0.56 |
| **KNN (Tuned)** | Best params via GridSearchCV | **~0.67** |
| **Voting Ensemble** | KNN + DecisionTree + LogisticRegression | **~0.70+** |

---

## 🌸 Insights & Highlights
💎 Scaling the data significantly improved performance  
💎 “Distance” weighting helped nearby samples influence predictions  
💎 Ensemble models boosted accuracy and overall stability  
💎 The model performs beautifully on real-world-like classification problems

---

## 🎨 Visualizations & Insights

### 🍇 1️⃣ Feature Correlation Heatmap
<img src="images/correlation_heatmap.png" width="700"/>

Shows relationships among chemical features of wine.  
**Insight:** Alcohol, density, and sulphates have strong correlation with wine quality.

---

### 🍷 2️⃣ Alcohol Content Distribution by Quality
<img src="images/alcohol_distribution.png" width="700"/>

Density plot comparing alcohol percentage in good vs. not-good wines.  
**Insight:** Good wines have noticeably higher alcohol levels.

---

### 💡 3️⃣ Top 10 Most Important Features (XGBoost)
<img src="images/xgboost_importance.png" width="700"/>

Feature importance scores ranked by XGBoost model.  
**Insight:** Alcohol, sulphates, and density are top predictors of wine quality.

---

### 📊 4️⃣ Confusion Matrices for KNN and XGBoost
<img src="images/confusion_knn.png" width="350"/> <img src="images/confusion_xgb.png" width="350"/>

Compares how well each model predicted correct vs. incorrect classifications.  
**Insight:** XGBoost achieved better precision and recall on “Good” wines.

---

### 📈 5️⃣ ROC–AUC Curve
<img src="images/roc_curve.png" width="700"/>

Illustrates trade-off between true positive and false positive rates.  
**Insight:** XGBoost achieved **AUC ≈ 0.90**, showing strong separability between good and not-good wines.

---

### 🔍 6️⃣ Precision–Recall Curve
<img src="images/pr_curve.png" width="700"/>

Demonstrates precision-recall relationship for both models.  
**Insight:** XGBoost maintains high precision even as recall increases — excellent for detecting “Good” wines.

---

### 💖 7️⃣ Accuracy Comparison Bar Plot
<img src="images/accuracy_comparison.png" width="600"/>

Side-by-side accuracy comparison between KNN and XGBoost.  
**Result:**  
🎯 KNN → ~79%  
⚡ XGBoost → ~85%

---

### 💎 8️⃣ Model Performance Radar Chart
<img src="images/radar_chart.png" width="600"/>

Summarizes **Accuracy**, **ROC–AUC**, and **PR–AUC** across models.  
**Insight:** XGBoost outperforms across all three dimensions.

---

### 🌈 9️⃣ Overall Takeaway
> 📊 Using data balancing, feature engineering, and boosted algorithms,  
> the final model achieved **85% accuracy with 0.90+ AUC**, proving that chemistry can indeed predict taste!

---

🖼️ *Note:*  
If you want these plots to show directly in your GitHub README:  
- Save each image from your notebook with:
  ```python
  plt.savefig("images/<plot_name>.png", dpi=300, bbox_inches="tight")


---

## 🌷 Next Steps
- Add **Random Forest or Gradient Boosting** comparisons 🌳  
- Build a **Streamlit / Gradio web app** for live predictions 💅  
- Expand to include **white wine** data 🍾  

---

## 👩🏽‍💻 Author
**Tenika Powell**  
💼 *Machine Learning Engineer in Training*  
📫 [Powell.tenika.n@gmail.com](mailto:Powell.tenika.n@gmail.com)  
💻 [GitHub – Nikkilabesf](https://github.com/Nikkilabesf)  
🌸 Passionate about AI, healthcare, and elegant code

---

## 💫 Final Thoughts
This project showcases how **data science can be both analytical and aesthetic**.  
With the perfect mix of algorithms, creativity, and curiosity —  
we turned chemistry into **AI-powered taste testing** 🍷💖

<p align="center">✨ Data. Beauty. Precision. ✨</p>
