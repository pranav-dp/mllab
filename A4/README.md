# Assignment 4: Binary Classification (SVM & Logistic Regression)

## 🎯 Objective

Classify emails as **Spam** or **Ham** using **Logistic Regression** and **Support Vector Machines** with different kernels and hyperparameter optimization.

## 📁 Structure

```
A4/
├── dataset/
│   └── spambase_csv.csv
├── notebooks/
│   ├── experiment4.ipynb
│   └── results_exp4.txt
├── plots/
│   └── eps/              # EPS plots
├── png/                  # PNG plots
├── report.pdf
└── report.tex
```

## 📊 Dataset

- **Spambase Dataset**: 4,601 emails with 57 features
- **Features**: Word/character frequencies (e.g., "free", "money", "$", "!")
- **Target**: Binary (1=Spam, 0=Ham)

## 🤖 Models Implemented

1. **Logistic Regression**: Optimized C, penalty (L1/L2), solver
2. **SVM Kernels**: Linear, Polynomial, RBF, Sigmoid
3. **Hyperparameter Tuning**: GridSearchCV for optimal parameters

## 📈 Results

### Best Model Performance
| Model | Accuracy | Precision | Recall | F1 Score | AUC |
|-------|----------|-----------|--------|----------|-----|
| **Logistic Regression** | 0.9262 | 0.9202 | 0.8898 | 0.9048 | 0.98 |
| **SVM (RBF)** | 0.9207 | 0.9143 | 0.8815 | 0.8976 | 0.98 |

### SVM Kernel Comparison
| Kernel | Accuracy | F1 Score | Training Time |
|--------|----------|----------|---------------|
| **Linear** | **0.9294** | **0.9093** | 0.41s |
| RBF | 0.9273 | 0.9055 | 0.22s |
| Sigmoid | 0.8849 | 0.8528 | 0.32s |
| Polynomial | 0.7796 | 0.6220 | 0.31s |

## 📊 Key Visualizations

- `class_distribution`: Target balance analysis
- `feature_correlation`: Feature importance heatmap
- `confusion_matrices`: Model performance comparison
- `roc_curve`: ROC-AUC analysis
- `learning_curve_*`: Bias-variance diagnostics

## 🚀 How to Run

```bash
cd A4
jupyter notebook notebooks/experiment4.ipynb
```