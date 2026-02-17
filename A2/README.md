# Assignment 2: Binary Classification (Naive Bayes & KNN)

## 🎯 Objective

Implement and compare Naive Bayes variants (Gaussian, Multinomial, Bernoulli) and K-Nearest Neighbors for binary spam classification.

## 📁 Structure

```
A2/
├── dataset/
│   └── spambase/
│       └── spambase_csv.csv
├── notebooks/
│   └── experiment2.ipynb
├── plots/
│   └── eps/              # EPS plots
├── png/                  # PNG plots
├── report.pdf
└── report.tex
```

## 📈 Dataset

- **Spambase Dataset**: 4,601 emails with 57 features
- **Task**: Binary classification (Spam vs Ham)
- **Features**: Word/character frequencies

## 🤖 Algorithms Implemented

1. **Naive Bayes**:
   - Gaussian NB
   - Multinomial NB
   - Bernoulli NB

2. **K-Nearest Neighbors**:
   - Hyperparameter tuning (k, algorithm)
   - Distance metrics comparison

## 📊 Key Visualizations

- `class_distribution`: Target variable balance
- `feature_distribution`: Feature histograms
- `confusion_matrices`: Model performance
- `roc_curves`: ROC-AUC comparison
- `knn_accuracy_vs_k`: Optimal k selection
- `learning_curve_*`: Bias-variance analysis

## 📈 Results Summary

- **Naive Bayes**: Fast training, good baseline performance
- **KNN**: Requires hyperparameter tuning, slower inference
- **Best Performance**: Gaussian NB for continuous features

## 🚀 How to Run

```bash
cd A2
jupyter notebook notebooks/experiment2.ipynb
```
