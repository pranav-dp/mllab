# Assignment 3: Regression Analysis (Loan Amount Prediction)

## 🎯 Objective

Predict **Loan Sanction Amount (USD)** using various linear regression models and analyze the impact of regularization techniques.

## 📁 Structure

```
A3/
├── dataset/
│   └── Predict Loan Amount Data/
│       ├── train.csv
│       └── test.csv
├── notebooks/
│   ├── experiment3.ipynb
│   └── results.txt
├── plots/
│   └── eps/              # EPS plots
├── png/                  # PNG plots
├── report.pdf
└── report.tex
```

## 📊 Dataset

- **Target**: Loan Sanction Amount (USD)
- **Key Features**: Loan Request, Income, Credit Score, Property Age, Profession
- **Task**: Regression with regularization

## 🤖 Models Implemented

1. **Linear Regression** - Baseline model
2. **Ridge Regression (L2)** - Handles multicollinearity
3. **Lasso Regression (L1)** - Feature selection
4. **Elastic Net** - Combined L1/L2 penalties

## 📈 Results

| Model | MAE | RMSE | R² Score |
|-------|-----|------|----------|
| Linear | 21,588 | 31,925 | 0.5510 |
| Ridge | 21,582 | 31,897 | 0.5517 |
| Lasso | 21,564 | 31,905 | 0.5515 |
| **Elastic Net** | **21,642** | **31,882** | **0.5522** |

## 📊 Key Visualizations

- `target_distribution`: Loan amount distribution
- `correlation_heatmap`: Feature relationships
- `predicted_vs_actual`: Model performance
- `residual_plot`: Error analysis
- `coefficients_comparison`: Regularization effects
- `learning_curve_*`: Bias-variance diagnostics

## 🚀 How to Run

```bash
cd A3
jupyter notebook notebooks/experiment3.ipynb
```