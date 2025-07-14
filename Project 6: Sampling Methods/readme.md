# Project 6: Sampling Methods

Implement two sampling-based inference methods: rejection sampling for a Gaussian Mixture Model (GMM), and MCMC (via Metropolis) for Bayesian linear regression.

---

## Part 1 — Rejection Sampling on GMM (1-D)

- Use the same 1-D Gaussian mixture model from **Project 5 (EM)**.
- Proposal distribution: standard normal
- Implement rejection sampling to draw samples from the GMM
- Plot:
  - Histogram of the accepted samples
  - True GMM PDF overlaid for comparison

---

## Part 2 — Bayesian Linear Regression via MCMC

- Reuse the training data generation code from **Project 2** (25 samples)
- Use Equation 3.10 (Gaussian likelihood on targets) as the likelihood:
  - p(t | w) = N(t | Φw, β⁻¹ I)
- Choose a prior for the weights (e.g., standard normal)
- Define the posterior:
  - posterior ∝ likelihood × prior
- Work in **log-space** for numerical stability
- Implement the **Metropolis algorithm** (Equation 11.33 from PRML) to sample from the posterior over weights
- Use the samples to estimate the mean of the posterior distribution of the weights
- Plot:
  - Trace plots of each weight over MCMC iterations
  - Histogram or KDE of the posterior samples
  - Predictive mean line from the posterior mean weights

---

## Stretch Goal

- Draw samples from the **posterior predictive distribution**
- Use samples of weights \( w^{(i)} \sim p(w \mid \text{data}) \) to draw:
  - \( t^{(i)} \sim p(t^* \mid x^*, w^{(i)}) \)
- Plot:
  - Predictive mean with confidence bands (e.g., 5th to 95th percentile)
  - Overlay predictions on top of the original training data

For reference on the predictive sampling procedure, see:  
https://stats.stackexchange.com/questions/185311/why-does-sampling-from-the-posterior-predictive-distribution-px-new-mid-x-1
