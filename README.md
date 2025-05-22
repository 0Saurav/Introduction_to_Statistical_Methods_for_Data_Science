# Introduction to Statistical Methods for Data Science

This repository contains the complete coursework for the subject **"Introduction to Statistical Methods for Data Science"**, focusing on modeling and inference using real-world energy data from a Combined Cycle Power Plant (CCPP).

---

## 📂 Dataset Overview

The dataset consists of the following variables:

- `x1` – Ambient Temperature
- `x2` – Net hourly electrical energy output (target variable)
- `x3` – Ambient Pressure
- `x4` – Relative Humidity
- `x5` – Exhaust Vacuum

---

## ✅ Task 1: Preliminary Data Analysis

1. **Time Series Plots**:  
   Visualized all input variables (`x1`, `x3`, `x4`, `x5`) and the output variable (`x2`) over time.

2. **Distribution Analysis**:  
   Plotted histograms and density plots to assess **skewness and normality** of variables.

3. **Correlation & Pairwise Plots**:  
   - Created a **correlation matrix**.
   - Generated scatter plots to explore relationships, especially with the target variable `x2`.

---

## ✅ Task 2: Regression Modeling

For **five different regression models**, the following steps were performed:

### 2.1 Parameter Estimation
- Estimated model parameters using **Least Squares (LS)**.

### 2.2–2.4 Model Comparison Metrics
- Computed **Residual Sum of Squares (RSS)**.
- Calculated **Log-Likelihood** for each model.
- Derived **AIC** and **BIC** values for model selection.

### 2.5 Residual Diagnostics
- Plotted **Q-Q plots** for residuals to assess **normality** and detect **outliers or skew**.

### 2.6 Model Selection
- Compared all models using AIC, BIC, and diagnostic plots.
- Selected the **best-performing model**.

### 2.7 Prediction with Uncertainty
- **Split** the dataset into **70% training** and **30% testing**.
- Trained the best model and made predictions on the test set.
- Constructed **95% confidence intervals** around predictions.

---

## ✅ Task 3: Approximate Bayesian Computation (ABC)

Implemented ABC to estimate posterior distributions of two influential parameters from the best model:

1. **Parameter Selection**:  
   Selected 2 most influential parameters based on significance.

2. **Prior Specification**:  
   Defined **Uniform priors ±20%** around LS estimates.

3. **Posterior Estimation**:  
   Used **Rejection Sampling** to generate samples from the posterior.

4. **Posterior Visualization**:  
   - **2D joint posterior plot**
   - **1D marginal posterior plots** for each parameter

5. **Interpretation**:  
   Analyzed posterior shapes and compared with frequentist estimates.

---

## 📊 Output Files

- 📄 `Introduction_to_Statistical_Methods_for_Data_Science.Rmd` – All R code and analysis steps.
- 📁 Plots and summaries (available inside the R Markdown or rendered HTML).
- 📊 Data file (optional, if uploaded): `dataset.csv`

---

## 🧠 Tools Used

- R & RStudio
- `ggplot2`, `GGally`, `abc`, `stats`, `dplyr`, `gridExtra`, `caret`, etc.

---

## ✍️ Author

**Saurav Sen**  
Master’s in Data Science  
GitHub: [@0Saurav](https://github.com/0Saurav)

---

## 📌 Note

This repository is for academic and educational purposes. Results and interpretations are based on standard statistical practices applied to real-world data.

