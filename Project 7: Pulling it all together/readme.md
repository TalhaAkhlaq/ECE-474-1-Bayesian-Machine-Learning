# Project 7: Pulling It All Together

Read the assigned paper on **Gibbs Sampling** and implement the model described using a probabilistic programming framework.

## Main Task

- Use any probabilistic programming package such as:
  - PyMC
  - Stan / PyStan
  - NumPyro
- Reproduce the inference problem described in the Gibbs sampling paper
- If exact Gibbs sampling is not supported by the framework, use any available sampling method (e.g., NUTS, HMC, Metropolis)
- Perform inference and analyze the posterior distribution of the model parameters
- Plot:
  - Posterior trace plots
  - Posterior distributions (e.g., histograms or KDE)
  - Any relevant model diagnostics (e.g., R-hat, ESS)

## Stretch Goal

- Implement **Gibbs sampling manually**, as shown in the paper
- Use conditional distributions to iteratively sample each parameter
- Generate posterior samples and compare results to your framework-based implementation
