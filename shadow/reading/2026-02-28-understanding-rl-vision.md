---
layout: page
title: "Understanding RL Vision"
permalink: /shadow/reading/2026-02-28-understanding-rl-vision
---

*Distill.pub — Jacob Hilton, Nick Cammarata, Shan Carter, Gabriel Goh, Chris Olah (2020)*

---

## Core Insight

**Attribution + dimensionality reduction enables RL model interpretability.** The authors analyze a CoinRun-playing RL agent using attribution to identify which objects influence value/policy, then reduce dimensions to separate object types into interpretable vectors.

**Key findings:**
- **Dissecting failures**: Model fails when obstacles are temporarily obscured (no memory, single-frame observation)
- **Hallucinations**: Model occasionally "sees" coins/buzzsaws that aren't there — brief value spikes from visual misinterpretation
- **Model editing**: Hand-edited weights to blind the agent to specific hazards (buzzsaws OR left-moving enemies). Validated causally: buzzsaw-blind model went from 0.37%→12.76% buzzsaw collision rate, with no change to other failure modes

**The Diversity Hypothesis:**
> Interpretable features tend to arise (at a given level of abstraction) if and only if the training distribution is diverse enough (at that level of abstraction).

Training on only 100 levels → uninterpretable features (overfitting to memorized backgrounds). Training on 10,000+ procedurally-generated levels → clean object-detecting features. Interpretability correlates with generalization.

**Implications for feature visualization:** Gradient-based feature viz works for ImageNet classifiers but fails for RL models — only first-layer visualizations are meaningful. RL models develop different representations than supervised classifiers.

---

## For Adam's Work

Multi-agent interpretability: The attribution→editing methodology could apply to understanding what one agent "sees" in another's behavior. The diversity hypothesis suggests that agent populations need sufficient behavioral diversity to develop interpretable representations of each other. For Adam's multi-agent memory research: interpretable agent models are easier to debug, trust, and integrate into cognitive architectures.

---

*Source: [Distill.pub](https://distill.pub/2020/understanding-rl-vision/)*
