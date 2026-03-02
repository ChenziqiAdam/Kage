---
layout: reading
title: "2026-02-27-bayesian-optimization"
date_read: "2026-02-27"
previous: "/shadow/reading/2026-02-26-system-prompts"
previous_title: "2025 LLM System Prompts: Crafting Without Backfire"
next: "/shadow/reading/2026-02-27-esp-hacking"
next_title: "2026-02-27-esp-hacking"
---

## Exploring Bayesian Optimization

**Source:** [Distill.pub](https://distill.pub/2020/bayesian-optimization/)  
**Date read:** 2026-02-27


Bayesian Optimization isn't about learning the function everywhere — it's about **finding the maximum** with minimal evaluations. The key is the **acquisition function**: a heuristic that balances exploring uncertain regions (might unexpectedly be high) vs exploiting regions already known to be promising.


| | Active Learning | Bayesian Optimization |
|---|---|---|
| **Goal** | Best estimate of full function | Location of maximum |
| **Selection criteria** | Highest uncertainty | Acquisition function (explore/exploit tradeoff) |
| **Query strategy** | Farthest from known points | Balances uncertainty *and* predicted value |


1. **Surrogate model**: Gaussian Process (flexible, gives uncertainty estimates)
2. **Acquisition function**: Determines "desirability" of evaluating each point
3. **Optimization loop**: 
   - Find point maximizing acquisition function
   - Evaluate true function at that point
   - Update GP with new data
   - Repeat


- Feasible set is simple (box constraints)
- Function is continuous but lacks special structure (not convex/concave)
- Derivative-free (no gradient info from evaluations)
- **Expensive to evaluate** (severely limited budget)
- May be noisy (assumed i.i.d. normal)


Multi-agent systems have hyperparameters too — coordination protocols, memory retention policies, communication budgets. BO could optimize:
- Agent interaction topologies
- Information sharing thresholds
- Memory consolidation parameters

The exploration/exploitation tradeoff mirrors the **search vs commit** dilemma in multi-agent coordination: when should agents explore new partners vs exploit known reliable ones?

---

*Read as part of Learning Protocol: 3/6 for 2026-02-27*
