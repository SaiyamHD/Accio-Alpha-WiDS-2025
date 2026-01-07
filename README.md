# Kalman Filtering & Quantitative Methods – Course Repository

This repository contains week-wise implementations and experiments covering probability fundamentals, statistical modeling, time-series analysis, and Kalman filtering. The work progresses from basic mathematical intuition and Python tooling to state estimation and filtering under uncertainty.

---

## Week 1 – Probability Foundations & Python Basics

### Focus
Building intuition for probability and setting up the Python ecosystem required for later weeks.

### Topics covered
- Basic probability concepts  
  - Random variables  
  - Mean, variance, standard deviation  
  - Gaussian (normal) distributions
- Intuition behind uncertainty and noise
- Numerical computation and visualization in Python

### Tools & libraries
- `numpy` for numerical operations
- `matplotlib` for plotting and visualization

### Outcome
- Comfort with Python for numerical experiments
- Ability to simulate and visualize noisy data
- Strong conceptual base for probabilistic modeling

---

## Week 2 – Statistical Modeling & Time-Series Analysis

### Focus
Applying probability and statistics to real datasets and financial time series.

### Key components
- Linear regression using Ordinary Least Squares (OLS)
- Interpretation of regression coefficients and interaction terms
- Confidence intervals and prediction intervals
- Diagnostic plots for regression models
- Stationarity analysis of time series
- Augmented Dickey–Fuller (ADF) test
- Mean reversion and half-life estimation
- Cointegration and spread construction for pairs trading

### Applications
- Salary prediction using multiple predictors
- Auto dataset analysis (`mpg` vs `horsepower`)
- Stationarity testing on USD/CAD price series
- Cointegration analysis of ETF pairs (EWA–EWC)

### Outcome
- Understanding when linear models are valid
- Ability to test stationarity and mean reversion
- Quantitative groundwork for state-space models

---

## Week 3 – Kalman Filter: Parameter Exploration & Extensions

### Focus
Understanding how Kalman filters behave under different assumptions and extending them to more realistic motion models.

### Parameter Exploration Tasks
Experiments performed on the provided Kalman filter implementation:

- Increase measurement noise (`R`) and observe behavior
- Increase process noise (`Q`) and observe behavior
- Start with very small initial uncertainty (`P`)
- Start with a very incorrect initial state and test recovery

### Coding Extensions
Implemented and analyzed:
- Extended state vector: **position + velocity**
- Tracking an object with **changing velocity**
- Adding **random acceleration** to true motion
- Comparison between:
  - Raw noisy measurements
  - Prediction-only estimates
  - Kalman Filter estimates

### Key insights
- Trade-off between responsiveness and smoothness
- Importance of realistic noise modeling
- Robustness of Kalman filters to poor initialization

### Outcome
- Practical understanding of Kalman filter tuning
- Clear intuition about model vs measurement trust
- Ability to design state-space models for dynamic systems

---
