---
title: Parameter Estimation in Hydrogen 21-cm Cosmology and MCMC Simulation
date: 2023-10-26
math: true

---

#  **Markov Chain Monte Carlo (MCMC) Simulations and Bayesian Inference**

##  Bayesian Inference and Motivation
Bayesian inference provides a systematic framework for **parameter estimation** by combining prior information with observational data.  
It allows us to:
1. Make **educated guesses** about model parameters.  
2. Quantify **uncertainty** in their possible values.  
3. Generate **predictions** by marginalizing over uncertainties.  
4. **Compare models** using evidences to determine which is more favorable.

The posterior probability is expressed as:

$$
P(\theta|D) = \frac{P(D|\theta) \, P(\theta)}{P(D)}
$$

where  
- $P(\theta|D)$ : Posterior probability of parameters given data,  
- $P(D|\theta)$ : Likelihood,  
- $P(\theta)$ : Prior,  
- $P(D)$ : Evidence (normalization factor).

---

##  MCMC — The Core Simulation Technique
The **Markov Chain Monte Carlo (MCMC)** method is a numerical approach to sample from complex posterior distributions when direct integration becomes computationally infeasible.  
It builds a *Markov chain* of parameter states where each new state depends only on the previous one — not the full history.

### Basic Idea
A Markov chain is a stochastic process where  
> *“What happens next depends only on the present state.”*  

MCMC algorithms, such as the **Metropolis–Hastings** or **Gibbs sampling**, are used to efficiently explore high-dimensional spaces by generating samples proportional to the target posterior distribution.

The **Metropolis–Hastings acceptance criterion** is:

$$
\alpha = \min \left(1, \frac{P(D|\theta') P(\theta')}{P(D|\theta) P(\theta)} \right)
$$

If $\alpha > \text{rand}(0,1)$, the new sample $\theta'$ is accepted; otherwise, the chain retains $\theta$.

---

##  Grid and Sampling Techniques
Earlier grid-based integrations suffered from the **curse of dimensionality** — computational costs growing exponentially with the number of parameters.  
MCMC overcomes this by sampling **only** the regions of high posterior probability, leading to more efficient estimation.

Improved convergence techniques use **Effective Sample Size (ESS)** and **adaptive proposals** to speed up convergence (see [Kish, 1965](https://en.wikipedia.org/wiki/Effective_sample_size)).



---

##  Goal of the project : Refining Bayesian Inference for 21-cm Cosmology
With [Dr. Raghunath Ghara](https://sites.google.com/view/raghunathghara/home) I am currently working on improving the **Bayesian inference framework** used in  
[“Constraints on the State of the IGM using LOFAR 21-cm Observations” (Ghara et al., 2025)](https://arxiv.org/abs/2505.00373).

The original analysis used uniform priors within a **COBAYA**-based MCMC pipeline to constrain intergalactic medium (IGM) parameters during the **Epoch of Reionization (EoR)**.  
However, such priors can introduce **strong prior dependence**, potentially biasing credible intervals.

My current work focuses on:
1. Reducing **prior dependence** in the inference process.    
2.Testing alternative likelihood formulations to improve the precision of parameter estimation in EoR models.


---




<!--more-->
