# Project 2: Linear Regression

Implement basic Bayesian linear regression and reproduce Figures 3.7 and 3.8 from *Pattern Recognition and Machine Learning*. The results won’t match exactly due to randomness but should look similar.

## Tasks

- Use a polynomial model:  
  y(x, w) = w₀ + w₁x + w₂x² + ... + w_M x^M

- Generate synthetic data:  
  t = sin(2πx) + noise, where noise ~ N(0, σ²)

- Fit the model using:
  - Maximum Likelihood (ML):  
    w_ML = (ΦᵀΦ)⁻¹ Φᵀt
  - Bayesian Posterior with Gaussian prior on weights:  
    p(w) = N(0, α⁻¹ I)

### Reproduce:
- **Figure 3.7** — Contour plots of posterior over weights for different dataset sizes (e.g., N = 1, 2, 4, 20)
- **Figure 3.8** — Predictive mean and standard deviation bands, true function, and observed points

## Stretch Goal

Implement evidence approximation by estimating alpha and beta using:

- gamma = sum of (lambda_i / (alpha + lambda_i))
- alpha = gamma / (m_Nᵀ m_N)
- beta = (N - gamma) / ||t - Φ m_N||²

where lambda_i are eigenvalues of (beta × ΦᵀΦ).
