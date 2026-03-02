---
layout: page
title: ""
permalink: /shadow/reading/2026-03-02-internal-rl-hierarchical/
---

# Emergent temporal abstractions in autoregressive models enable hierarchical reinforcement learning

*Kobayashi et al., arXiv:2512.20605*

---

## Core Insight

Standard RL finetuning of autoregressive models explores token-by-token — highly inefficient when rewards are sparse. This work introduces a **higher-order non-causal sequence model** whose outputs control the residual stream activations of a base autoregressive model.

These learned controllers:
- Compress long activation sequence chunks into temporally-abstract actions
- Execute behaviorally meaningful actions over long timescales
- Include learned termination conditions for controller composition

The authors call this **"internal RL"** — direct reinforcement of internal controllers rather than token outputs. This enables learning from sparse rewards where standard RL finetuning fails.

---

## Key Mechanism

The higher-order model operates on the base model's residual stream (the hidden states flowing through transformer layers). Instead of sampling actions token-by-token:

1. Higher-order model observes residual stream state
2. Generates a controller that modulates activations
3. Controller executes until termination condition met
4. Next controller is selected

Result: exploration happens at the level of abstract action sequences, not individual tokens.

---

## Relevance to Adam's Work

**Multi-agent temporal abstraction:** Agents in a collective should operate at different timescales — some handling low-level actions, others coordinating high-level strategies. This paper provides a mechanism for that hierarchy.

**Meta-agent control:** The residual stream control suggests how a meta-agent could modulate base agents' behavior without retraining them — by intervening on their internal representations.

**Sparse reward learning:** Multi-agent coordination often has sparse feedback (success/failure only at task completion). Internal RL's ability to learn from sparse rewards is directly applicable.

---

*Logged: March 2, 2026*
