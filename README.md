# Portfolio Optimization in Python 

This repository contains a series of academic projects exploring asset allocation and portfolio theory. The notebooks progress from calculating basic historical risk metrics to applying convex optimization for portfolio weighting. 

## Repository Contents

### **Assignment 1: Financial Data & Risk Metrics**
* **Concepts:** Log returns, annualized volatility, covariance, and correlation.
* **Description:** Fetches historical stock data using `yfinance` to calculate standard risk and return metrics. Includes a simple script to identify negatively correlated asset pairs.

### **Assignment 2: Portfolio Geometry & The Efficient Frontier**
* **Concepts:** Long-only constraints, risk-return clouds, minimum variance portfolio.
* **Description:** Uses a basic grid-search to generate feasible portfolio weight combinations. Visualizes the "Risk Surface" heat map and plots the Efficient Frontier over a risk-return scatter cloud. Includes a visual stress-test simulating increased asset correlation.

### **Assignment 3: Markowitz Mean-Variance Optimization**
* **Concepts:** Global Minimum Variance (GMV), target-return constraints.
* **Description:** Replaces the brute-force grid search with actual optimization using **CVXPY**. Computes the Efficient Frontier by minimizing quadratic risk for specific target returns, and compares the optimized portfolio against a simple equal-weight ($1/N$) portfolio.

### **Final Project: Modeling Investor Risk Aversion**
* **Concepts:** Utility theory, risk aversion parameter ($\lambda$), dynamic asset allocation.
* **Description:** An exercise showing how optimal weights change based on an investor's risk tolerance. By making Risk Aversion ($\lambda$) a tunable parameter, the script models how a portfolio mathematically transitions from high-risk equities to safer assets (like Treasury bonds) as the risk penalty increases.

## Tech Stack
* **Language:** Python 3
* **Libraries:** `yfinance`, `pandas`, `numpy`, `cvxpy`, `matplotlib`, `seaborn`
* **Environment:** Google Colab / Jupyter Notebooks

## How to Run
All files are provided as Jupyter Notebooks (`.ipynb`). 
1. Clone this repository or download the files.
2. Open them in [Google Colab](https://colab.research.google.com/) or your local Jupyter environment.
3. Run the cells sequentially. The notebooks will pull the required historical market data automatically via Yahoo Finance.
