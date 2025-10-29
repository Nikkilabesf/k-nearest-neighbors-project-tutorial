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

## 📈 Visual Outputs
🪄 Confusion Matrix (Heatmap)  
🌈 Accuracy vs k-Value Graph  
📉 Feature Correlation Matrix  

*(All plots are styled in soft color palettes for aesthetic visualization.)*

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
