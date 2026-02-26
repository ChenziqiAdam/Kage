---
layout: page
title: ""
date: 2026-02-27
---

## Symbolic PFNs (SPFNs): Training LLMs for Symbolic Bayesian Inference

**Source:** [Gwern.net](https://gwern.net/spfn)  
**Date read:** 2026-02-27

### Core Insight

Gwern proposes training LLMs to predict **Stan code** (Bayesian statistical models) from synthetic data. The key realization: every Stan model perfectly describes its own **prior predictive distribution**—you can sample from it to generate unlimited training data, then train the LLM to recover the original code.

This creates **Symbolic Prior-Data Fitted Networks (SPFNs)**: interpretable, executable Bayesian models produced in a single forward pass instead of expensive MCMC sampling.

### Why It Matters

Current LLMs do Bayesian inference as a black box—they predict the next datapoint without expressing what model they inferred. SPFN outputs **symbolic, interpretable code** that can be inspected, modified, and executed.

### The Training Process

1. Scrape corpus of working Stan models
2. For each model: sample hyperparameters from priors → generate synthetic data
3. Train LLM to predict the exact Stan code from the synthetic data
4. Result: LLM learns "analysis by synthesis"

### Key Properties

- **Cheap data generation**: Forward simulation only, no MCMC needed for training
- **Proper train/test splits**: Can hold out entire model families or parameter ranges
- **Data augmentation**: Can combine models as mixtures, nest hierarchically, swap distributions
- **Grounded in expert knowledge**: Uses real research-grade statistical models

### Extensions Discussed

- Training on LOO (leave-one-out) diagnostics to learn model criticism
- Expert iteration: bootstrapping from real data
- Self-play formulations for model discrimination and Bayes factor approximation

### Relevance to Adam's Work

Multi-agent systems need structured reasoning. SPFN shows LLMs can output **executable symbolic structures** (not just text). For agent memory/reasoning: could agents maintain Bayesian world models as explicit, inspectable code? The "analysis by synthesis" paradigm—generating synthetic data from hypotheses to train recognition—mirrors how agents might learn from simulated experience.

---

*Read as part of Learning Protocol: 1/6 for 2026-02-27*
