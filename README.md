# Credit Risk and Statistical Learning Project

## Project Overview
This project was developed as part of the **Quantitative Risk Management** course (FIN-417) at **EPFL** (Fall 2025). The objective is to model credit risk for retail loans using synthetic data. We implemented statistical learning techniques to predict repayment probabilities and evaluated the financial impact of different lending strategies using Monte Carlo simulations.

## Group Members
- **Matthias Wyss** (matthias.wyss@epfl.ch)
- **William Jallot** (william.jallot@epfl.ch)
- **Antoine Garin** (antoine.garin@epfl.ch)

## Key Features
- **Data Simulation**: Generation of synthetic borrower profiles based on age, income, and employment status.
- **Statistical Modeling**: Implementation and comparison of:
  - **Logistic Regression** (Linear baseline).
  - **Support Vector Machines (SVM)** with RBF kernels to capture non-linear default patterns.
- **Performance Metrics**: Evaluation using Cross-Entropy Loss, ROC Curves, and Area Under the Curve (AUC).
- **Risk Management**: Financial simulation of lending policies to calculate:
  - Expected Profit & Loss (PnL).
  - Value-at-Risk (VaR) at 95%.
  - Expected Shortfall (ES) at 95%.

## Repository Structure
- `pdfs/Report.pdf`: The final academic report detailing methodology, results, and analysis.
- `analysis.ipynb`: Jupyter Notebook containing the full Python implementation.
- `pdfs/Instructions.pdf`: The original project brief and constraints.

## Methodology Summary
The project highlights the importance of non-linear models when dealing with complex borrower behavior. While Logistic Regression performs well on linear datasets, the **SVM (RBF)** proved superior in scenarios where repayment probability depends non-linearly on features like age. We also demonstrated that selective lending based on high-probability thresholds (95%+) significantly improves the risk-return profile of a loan portfolio compared to "lend-to-all" strategies.

## Requirements
To run the notebook, you will need the following Python libraries:
- `numpy`
- `matplotlib`
- `scikit-learn`
- `scipy`

## Usage
1. Clone this repository.
2. Open `analysis.ipynb` in Jupyter Lab or Google Colab.
3. Run all cells to reproduce the figures and tables found in the report. (Note: A random seed `0` is set for reproducibility).

---
*Supervised by Dr. Urban Ulrych and Andrea Ruglioni - EPFL.*