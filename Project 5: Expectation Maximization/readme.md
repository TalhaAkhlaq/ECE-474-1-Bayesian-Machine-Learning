# Project 5: Expectation Maximization

Implement the Expectation-Maximization (EM) algorithm for a Gaussian Mixture Model (GMM) in both 1-D and 2-D.

## 1-D Gaussian Mixture Model

- Use K = 3 components.
- Choose your own initial values for:
  - Means (μ₁, μ₂, μ₃)
  - Variances (σ₁², σ₂², σ₃²)
  - Mixing coefficients (π₁, π₂, π₃)

- Follow EM steps as defined in Equations 9.23–9.28 from *Pattern Recognition and Machine Learning*.

- Generate a set of 1-D observations from your GMM.

- Plot:
  - A histogram of the data
  - The mixture density (PDF) overlaid
  - Show the initial PDF and how it evolves (e.g. at initialization, mid-training, convergence)

- Optional:
  - Make a movie showing the progression of the fit
  - Introduce a single data point exactly equal to one of the initial means to test convergence stability

## 2-D Gaussian Mixture Model

- Use K = 2 components
- Use the **Old Faithful** dataset (geyser eruption data)
- Plot:
  - Data points
  - Contour lines or ellipses of the Gaussian components
  - Similar to Figure 9.8 in *PRML*


