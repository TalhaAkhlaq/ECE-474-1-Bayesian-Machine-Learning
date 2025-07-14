# Project 4: Gaussian Processes and Kernel Methods

Reproduce the predictive plots from the second part of your linear regression assignment (Figure 3.8 from PRML), but this time using **Gaussian Processes** instead of a parametric model.

## Tasks

- Replace your linear model’s prediction equations (3.58 and 3.59) with the Gaussian Process equivalents (equations 6.66 and 6.67 from PRML).
- Use the **Gaussian (RBF) kernel**:
  k(x, x′) = exp(−(1/2ℓ²) * ||x − x′||²)  
  (PRML Equation 6.23)
- Build the full covariance matrix C using Equation 6.62:
  C = K(X, X) + σ² * I  
  where K is the kernel matrix and σ² is the noise variance
- Plot the GP predictive mean and ±1 standard deviation band along with the training data and the true function (as in Figure 3.8)

## Stretch Goal

- Read the paper: **A Practical Guide to Support Vector Classification**  
- On the same datasets from **Project 3**, implement the SVM grid search procedure described in the paper.
- Evaluate classification performance (accuracy, ROC curve) and compare to previous models.
