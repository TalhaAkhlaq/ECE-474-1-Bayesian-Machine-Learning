# Conjugate Estimators

## Scenarios
| Scenario | Likelihood | Conjugate Prior | Parameter |
|----------|------------|-----------------|-----------|
| Binomial | **Binomial** \((n, p)\) | **Beta** \((\alpha, \beta)\) | \(p\) |
| Gaussian, known variance | **Normal** \((μ, σ²)\) | **Normal** \((μ₀, τ²)\) | \(μ\) |
| Gaussian, known mean | **Normal** \((μ, σ²)\) | **Inverse-Gamma** \((a, b)\) | \(σ²\) |

## Tasks
1. **MSE Comparison**  
   * Simulate data for each scenario.  
   * Compute maximum-likelihood and Bayesian posterior-mean estimates.  
   * Select **2–3** distinct hyper-parameter settings per prior.  
   * Plot mean-squared error curves for both estimators on one figure with a legend.

2. **Posterior Evolution**  
   * For at least one hyper-parameter choice per scenario, plot the posterior density after multiple observation counts (for example, \(k = 1, 5, 20, 100\)) to show convergence.

## Stretch Goals
* **Posterior Animation** — Create an animation illustrating posterior updates as observations accumulate.  
* **Unknown \(μ, σ²\) Case** — Use the **Normal-Inverse-Gamma** prior to infer both parameters jointly and visualize the evolving joint posterior with heatmaps or contour plots.
