# ML-Algorithms
Python implementations of ML algorithms — preprocessing, classification, regression, clustering

# Sleep Health Prediction — ML Study

A hands-on exploration of machine learning applied to sleep health data. The goal was to predict two things from a person's daily habits and health indicators:

- **Sleep Disorder** (Classification) — No Disorder, Insomnia, or Sleep Apnea
- **Quality of Sleep** (Regression) — score from 1 to 10

Each algorithm gets its own notebook, fully self-contained, so you can jump to any one directly.

---

## Dataset

**Sleep Health and Lifestyle Dataset** 
— [Kaggle](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset)



## Notebooks

| # | Notebook | What it does |
|---|----------|--------------|
| 00 | `00_Preprocessing.ipynb` | Data cleaning, encoding, exploration |
| 01 | `01_Linear_Regression.ipynb` | Predicts sleep quality score |
| 02 | `02_Polynomial_Regression.ipynb` | Same target, adds polynomial features |
| 03 | `03_Logistic_Regression.ipynb` | Classifies sleep disorder |
| 04 | `04_KNN.ipynb` | KNN classifier, tunes K |
| 05 | `05_SVM.ipynb` | SVM with RBF kernel |
| 06 | `06_Decision_Tree.ipynb` | Decision tree with depth tuning |
| 07 | `07_Random_Forest.ipynb` | Random forest, feature importance |
| 08 | `08_Model_Comparison.ipynb` | Runs all models, compares metrics, picks the best |

---

## Results

**Regression (Quality of Sleep)**

| Model | R² | RMSE |
|-------|----|------|
| Linear Regression | **0.9629** | 0.2367 |
| Polynomial Regression | 0.9325 | 0.3191 |

**Classification (Sleep Disorder)**

| Model | Accuracy | F1 |
|-------|----------|----|
| Logistic Regression | **0.88** | 0.8806 |
| KNN (K=8) | 0.8667 | 0.8643 |
| SVM (RBF) | 0.8533 | 0.8555 |
| Decision Tree | 0.88 | 0.8763 |
| Random Forest | 0.88 | 0.8785 |

Linear Regression came out on top for sleep quality (R²=0.96), and Logistic Regression tied with Decision Tree and Random Forest for disorder classification at 88% accuracy.


