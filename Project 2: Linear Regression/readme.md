# Project 2: Linear Regression

Implement basic Bayesian linear regression and reproduce Figures 3.7 and 3.8 from *Pattern Recognition and Machine Learning*. The figures won't match exactly due to randomness but should be visually similar.

## Tasks

- Use a polynomial model:
  \[
  y(x, \mathbf{w}) = \sum_{j=0}^M w_j x^j
  \]
- Generate data:
  \[
  t = \sin(2\pi x) + \varepsilon,\quad \varepsilon \sim \mathcal{N}(0, \sigma^2)
  \]
- Fit using:
  - **ML estimate**:
    \[
    \mathbf{w}_{\text{ML}} = (\Phi^\top \Phi)^{-1} \Phi^\top \mathbf{t}
    \]
  - **Bayesian posterior** with prior \( \mathcal{N}(0, \alpha^{-1} \mathbf{I}) \)

### Reproduce:
- **Figure 3.7** — Posterior over weights for different dataset sizes  
- **Figure 3.8** — Predictive mean, variance, and true function

## Stretch Goal

Implement the evidence approximation using:
\[
\alpha = \frac{\gamma}{\mathbf{m}_N^\top \mathbf{m}_N},\quad
\beta = \frac{N - \gamma}{\| \mathbf{t} - \Phi \mathbf{m}_N \|^2}
\]
where
\[
\gamma = \sum_i \frac{\lambda_i}{\alpha + \lambda_i}
\]
and \( \lambda_i \) are eigenvalues of \( \beta \Phi^\top \Phi \).
