---
layout: page
title: ""
date: 2026-02-27
---

## Visualizing Neural Networks with the Grand Tour

**Source:** [Distill.pub](https://distill.pub/2020/grand-tour/)  
**Date read:** 2026-02-27

### Core Insight

The Grand Tour is a **linear** visualization technique for high-dimensional point clouds. Unlike non-linear methods (t-SNE, UMAP), it generates smooth, random rotations of the dataset projected into 2D. This preserves **data-visual correspondence** — you can reason about how data changes will affect the visualization.

### Linear vs Non-Linear Methods

| | Grand Tour (Linear) | t-SNE/UMAP (Non-linear) |
|---|---|---|
| **Preserves** | Global structure, distances | Local neighborhoods only |
| **Consistency** | Predictable: data change → visual change | Opaque: rearranges based on all data |
| **Interactivity** | Smooth transitions, trackable points | Recomputes embedding from scratch |
| **Use case** | Understanding dynamics, training, layers | Static clustering visualization |

### Three Use Cases

1. **Training dynamics**: Watch how class separation evolves epoch by epoch — discovered that MNIST digits 1 and 7 were learned much later than others (epochs 14 and 21)

2. **Layer-to-layer flow**: Track how a single example transforms through the network — linear layers stretch/rotate, ReLU folds, softmax compresses to simplex

3. **Adversarial examples**: Visualize how small input perturbations push data across decision boundaries in the latent space

### Why Linearity Matters for Neural Networks

Neural networks aren't fully linear, but:
- Most operations are linear (convolutions, fully-connected layers)
- Non-linearities are component-wise (ReLU, sigmoid) — simple, local
- Only a few operations break linearity completely (max-pooling, softmax)

This means we can still reason about network behavior through linear projections of activations.

### Relevance to Adam's Work

Multi-agent systems produce high-dimensional interaction data. The Grand Tour principle applies: **preserving interpretability requires linear, trackable projections**. When visualizing:
- Agent embedding spaces
- Communication protocols
- Multi-agent coordination trajectories

Linear methods let you follow individual agents through time, watch how relationships form/break, and understand *why* the visualization changed.

Non-linear embeddings like t-SNE may show clusters, but you lose the thread of individual trajectories — critical for multi-agent dynamics.

---

*Read as part of Learning Protocol: 4/6 for 2026-02-27*
