<!-- hide -->
# K-Nearest Neighbors - Step-by-Step Guide
<!-- endhide -->

- Understand a new dataset.
- Model the data using a KNN.
- Analyze the results and optimize the model.

<how-to-start>

## 🌱 How to start this project

Follow these instructions:

1. Create a new repository based on the [Machine Learning project](https://github.com/4GeeksAcademy/machine-learning-python-template) [by clicking here](https://github.com/4GeeksAcademy/machine-learning-python-template/generate).
2. Open the newly created repository in Codespace using the [Codespace button extension](https://docs.github.com/en/codespaces/developing-in-codespaces/creating-a-codespace-for-a-repository#creating-a-codespace-for-a-repository).
3. Once the Codespace's VSCode has finished opening, start your project by following the instructions below.

</how-to-start>

## 📝 Instructions

### Wine Classifier with KNN

Train a K-Nearest Neighbors (KNN) model to predict the quality of red wine based on its chemical properties. Could AI help you choose a sommelier-worthy wine?

We will use the following red wine dataset extracted from [Wine Quality Data Set - UCI](https://archive.ics.uci.edu/dataset/186/wine+quality)

```text
https://raw.githubusercontent.com/4GeeksAcademy/k-nearest-neighbors-project-tutorial/refs/heads/main/winequality-red.csv
```

#### Column Description

Each row represents a wine. The columns describe its chemical composition:

- fixed acidity, volatile acidity, citric acid

- residual sugar, chlorides

- free sulfur dioxide, total sulfur dioxide

- density, pH, sulphates, alcohol

The target column is **label**:

- 0 = Low quality

- 1 = Medium quality

- 2 = High quality

### Let's get started! 😎

1. **Load the data.** Load the CSV with Pandas and explore its structure.
2. **Train the KNN model:**
    - Separate the independent variables (X) from the target (y).

    - Split into training and testing sets (80/20).

    - Scale the data if necessary (highly recommended with KNN!).

    - Train the model with an initial k value.

3. Evaluate performance using:

    - `accuracy_score`

    - `confusion_matrix`

    - `classification_report`

4. **Optimize k.** Create a loop to test different k values (e.g., from 1 to 20).

    - Save the results in a list.

    - Plot accuracy vs k to find the best value.

## Feeling confident?

Create a function that takes numerical values and predicts the quality:

```python
predict_wine_quality([7.4, 0.7, 0.0, 1.9, 0.076, 11.0, 34.0, 0.9978, 3.51, 0.56, 9.4])
>>> "This wine is likely of medium quality 🍷"
```

> Note: We also provide solution samples in `./solution.ipynb`, which we honestly suggest you only use if you're stuck for more than 30 minutes or if you've already finished and want to compare it with your approach.

## 🚀 Make Your Work Visible

You worked with a real dataset from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/186/wine+quality), applied supervised classification models, analyzed chemical features, and developed a function that **simulates a sommelier's judgment using AI**. That deserves to be shared!

### What to Share?

Share an **insightful phrase** that demonstrates how AI can classify wine quality based on its composition. Add a precision vs. k plot (very visual) or a fun prediction using `predict_wine_quality()`.

---

### ✨ Postable Example

> **"Can artificial intelligence predict the quality of wine? 🍷 I trained a KNN model with real data from the UCI ML Repo and achieved 73% accuracy in classifying wines as low, medium, or high quality using only their chemical composition. The data doesn't lie: alcohol and sulfate are more revealing than a label! 😉 #MachineLearning #DataScience #WineLovers #AI #scikitLearn"**

## 🚛 How to deliver this project

Once you have finished solving the case study, make sure to commit your changes, push to your repository, and go to 4Geeks.com to submit the repository link.
