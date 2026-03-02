# Linear Regression — From Scratch & With Scikit-Learn



A comprehensive, educational deep-dive into **Linear Regression** — one of the most fundamental algorithms in machine learning and statistics. This project walks through the full theory, derives the math from first principles, implements the algorithm from scratch in Python, evaluates the model with standard metrics, validates the underlying assumptions, and cross-checks everything against scikit-learn.

---

## Table of Contents

- [Overview](#overview)
- [What You'll Learn](#what-youll-learn)
- [Project Structure](#project-structure)
- [Key Results](#key-results)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Author](#author)

---

## Overview

Linear regression is a supervised machine-learning algorithm that models the relationship between a dependent variable and one or more independent variables by fitting a linear equation to observed data. Despite its simplicity, it is the foundation for many advanced techniques (logistic regression, neural networks, etc.) and remains one of the most widely used tools in data science.

This notebook is designed to go beyond simply calling a library function — it aims to build genuine understanding of:

- **Why** the algorithm works the way it does
- **How** the coefficients are derived using calculus (minimizing the Sum of Squared Errors via partial derivatives)
- **What** the evaluation metrics actually mean
- **When** the model can (and cannot) be trusted, through assumption testing

---

## What You'll Learn

1. **Theory & Mathematics**
   - The linear regression equation: $\hat{Y} = \beta_0 + \beta_1 X + \varepsilon$
   - Cost function: Sum of Squared Errors (SSE)
   - Derivation of the slope ($\beta_1$) and intercept ($\beta_0$) using partial derivatives
   - Intuition behind the slope as the ratio of covariance to variance

2. **From-Scratch Implementation**
   - Generating synthetic data with NumPy
   - Computing the regression coefficients manually
   - Building a prediction function
   - Visualizing the data and the best-fit regression line

3. **Model Evaluation**
   - **MSE** (Mean Squared Error) — quantifies average squared prediction error
   - **RMSE** (Root Mean Squared Error) — interpretable average error in original units
   - **R²** (Coefficient of Determination) — proportion of variance explained by the model (~94% in this project)

4. **Assumption Testing**
   - **Linearity** — residuals vs. fitted values plot
   - **Independence of errors** — residuals vs. independent variable plot
   - **Normality of residuals** — histogram of error distribution
   - Discussion of homoscedasticity, multicollinearity, and endogeneity

5. **Scikit-Learn Validation**
   - Reproducing the same model using `sklearn.linear_model.LinearRegression`
   - Confirming that the from-scratch implementation matches scikit-learn's results

---

## Project Structure

```
Linear Regression/
├── Linear_regression.ipynb   # Main Jupyter Notebook (full analysis)
├── Linear-Regression.png     # Explanatory diagram
└── README.md                 # This file
```

---

## Key Results

| Metric | From Scratch | Scikit-Learn |
|--------|:------------:|:------------:|
| Intercept ($\beta_0$) | 0.9389 | 0.9389 |
| Slope ($\beta_1$) | 2.0180 | 2.0180 |
| MSE | 2.1526 | 2.1526 |
| RMSE | 1.4672 | 1.4672 |
| R² | 0.9405 | 0.9405 |

The model explains approximately **94%** of the variance in the target variable, confirming a strong linear relationship. The from-scratch implementation produces results identical to scikit-learn, validating the mathematical derivations.


---



## Author

**Andres Felipe Cruz**

Any feedback is always welcome, thanks for looking at my projects
