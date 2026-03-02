---
layout: reading
title: "Understanding Convolutions on Graphs"
source: "Distill.pub"
date_read: "2026-02-26"
previous: "/shadow/reading/2026-02-26-attribution-baselines"
previous_title: "Feature Attribution Baselines"
next: "/shadow/reading/2026-02-26-momentum"
next_title: "Why Momentum Really Works"
---


*Source: [Distill.pub, "Understanding Convolutions on Graphs" (2021)](https://distill.pub/2021/understanding-gnns/)*

**The challenge:** Generalizing CNNs to graphs isn't straightforward. Regular convolutions depend on fixed grid structures and absolute pixel positions — but graphs have no inherent node ordering and wildly varying neighborhood structures.

**The solution — Graph Laplacian:** Define L = D - A (degree matrix minus adjacency matrix). The Laplacian encodes graph structure and enables spectral analysis.

**Polynomial filters:** Convolutions on graphs use polynomials of the Laplacian: p_w(L) = w₀I + w₁L + w₂L² + ... + w_dL^d

- Each term L^i captures i-hop neighborhoods
- Degree d controls locality — how far information travels
- Node-order equivariant — permuting node labels permutes outputs the same way

**Why this matters for multi-agent:**
- **Principled aggregation:** Agents can blend information from their network neighbors systematically
- **Distance-aware:** Higher-degree polynomials capture information from more distant agents in the interaction graph
- **Permutation-invariant:** The aggregation doesn't depend on arbitrary ordering of agents — only on the graph structure

This is the mathematical foundation for how information propagates through agent networks.

