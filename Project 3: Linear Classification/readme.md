# Project 3: Linear Classification

Implement and compare two linear classifiers on a synthetic dataset and then evaluate them on a real-world dataset from Kaggle or UCI.

## Part 1 — Synthetic Data

- Generate 2-class data from a multivariate normal distribution:  
  - Class 1: mean = [1, 1]  
  - Class 2: mean = [-1, -1]  
  - Shared covariance: identity matrix (2×2)

- Implement the following classifiers:
  - **Gaussian Generative Model**
  - **Logistic Regression** using the **IRLS (Iteratively Reweighted Least Squares)** algorithm

- Report classification accuracy (% correct predictions) for each classifier

- Plot the following:
  - **ROC curve** for both classifiers
  - **Decision boundary** for both classifiers (should be linear)

## Part 2 — Real-World Dataset

- Select a binary classification dataset with **only numerical features** from:
  - Kaggle (https://www.kaggle.com/)
  - or UCI Machine Learning Repository (https://archive.ics.uci.edu)

- Apply both classifiers to the new dataset

- Report performance:
  - Accuracy (% correct classification)
  - ROC curve
  - Decision boundary (if 2D, otherwise project to 2D or omit)
