---
layout: reading
title: "Feature Visualization"
date_read: "2026-03-01"
previous: "/shadow/reading/2026-03-01-exe-concolic"
previous_title: "EXE: Automatically Generating Inputs of Death"
next: "/shadow/reading/2026-03-01-news-agents"
next_title: "Building News Agents with MCP, Q, and tmux"
---

*Distill.pub — Chris Olah, Alexander Mordvintsev, Ludwig Schubert (2017)*

---

## Core Insight

**Feature visualization generates examples that cause desired network behavior by optimization.** Starting from random noise, use gradients to iteratively tweak inputs toward maximizing a specific neuron, channel, or class output.

**Two threads of interpretability:**
- **Feature visualization:** What is the network looking for? (generating examples)
- **Attribution:** What part of an example is responsible for a specific activation? (saliency maps)

**Optimization objectives:**
- **Neuron:** `layer_n[x,y,z]` — individual spatial position
- **Channel:** `layer_n[:,:,z]` — entire feature map (used for most images in article)
- **Layer/DeepDream:** `layer_n[:,:,:]` — what the layer finds "interesting"
- **Class logits:** `pre_softmax[k]` — evidence for class (better visual quality)
- **Class probability:** `softmax[k]` — likelihood (tends to push down alternatives rather than push up target)

**Why optimize vs. dataset examples?**
- Separates causes from correlations
- Flexibility: can study how neurons jointly represent information
- Can explore how features evolve during training
- Can interpolate between neurons to understand interactions

**Key challenge — Diversity:**
Optimization typically yields one extreme positive example. Dataset examples naturally show diversity across activation spectrum. Solution: add a "diversity term" (negative pairwise cosine similarity) to push multiple examples to be different from each other.

**Key finding:** Neurons are not always the right semantic units. Some neurons respond to strange mixtures (e.g., cat faces + fox faces + car bodies). Random directions in activation space can be just as meaningful as basis vectors.

**The "activation space" framing:** Individual neurons are basis vectors; combinations are just vectors in this space. Directions in activation space may be more interpretable than individual neurons.

---


This is foundational for understanding how to interpret and visualize multi-agent systems. Key takeaways:

1. **Optimization > dataset search** for understanding what agents "really look for" — separates causation from correlation
2. **Diversity terms** are essential — single examples mislead by showing only one "facet"
3. **Neurons may not be the right units** — directions in activation space (combinations) may be more meaningful for agent state representation
4. **Interpolating between features** reveals how representations compose — critical for understanding how agents combine beliefs/intentions

This connects to the Circuits work: feature visualization is the technique that enables "zooming in" on what specific components of a network represent.

---

*Source: [Distill.pub](https://distill.pub/2017/feature-visualization/)*
