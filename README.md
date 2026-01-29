# Image-Denosing-and-Sampling

## Overview
This repository explores **probabilistic inference and sampling methods** through a set of applied experiments on image denoising and latent-variable models. The project focuses on understanding how different inference techniques behave in practice, with particular emphasis on **approximate inference, convergence behavior, and qualitative results**.

The implementations are written in Python and organized as executable notebooks for clarity and reproducibility.

---

## Methods Covered

### 1. Image Denoising via Loopy Belief Propagation
- Binary image denoising using **max-product Loopy Belief Propagation**
- Pixels are modeled as binary random variables (`{-1, +1}`) on a grid graph
- Pairwise Markov Random Field with tunable coupling strength
- Experiments on:
  - Message passing dynamics
  - Momentum / damping in belief propagation
  - Effect of noise level and coupling strength on denoising quality

---

### 2. Markov Chain Monte Carlo in the TrueSkill Model
- Probabilistic modeling of player skills using a simplified **TrueSkill-style latent variable model**
- Likelihood based on logistic win probability
- Analysis of posterior distributions under different game outcomes
- Visualization of prior and posterior geometry

**Inference techniques:**
- Exact posterior visualization (low-dimensional cases)
- Sampling-based approximation

---

### 3. Hamiltonian Monte Carlo (HMC)
- Implementation of **Hamiltonian Monte Carlo** using leapfrog integration
- Sampling from posterior distributions over latent skills
- Comparison of posterior geometry and sample efficiency

---

### 4. Langevin Monte Carlo (LMC)
- Unadjusted and Metropolis-adjusted **Langevin Monte Carlo**
- Applied to both toy problems and real-world datasets
- Trade-off between computational efficiency and sampling bias

