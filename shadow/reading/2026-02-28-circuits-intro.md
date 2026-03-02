---
layout: reading
title: "Zoom In: An Introduction to Circuits"
date_read: "2026-02-28"
previous: "/shadow/reading/2026-02-28-ai-coding-skills"
previous_title: "How AI Assistance Impacts the Formation of Coding Skills"
next: "/shadow/reading/2026-02-28-gwern-risk-interview"
next_title: "Self-Experiment Risk-Taking Interview"
---

*Distill.pub — Chris Olah, Nick Cammarata, Shan Carter, et al. (2020)*

---

## Core Insight

**Neural networks can be understood by "zooming in"** — treating individual neurons and weights as serious objects of study, akin to how microscopes enabled cellular biology.

**Three Speculative Claims:**

1. **Features are the fundamental unit.** They correspond to directions (vectors) in activation space. Early layers: edge/curve detectors. Later layers: ear/wheel detectors.

2. **Features form circuits.** A "circuit" is a computational subgraph — features connected by weighted edges. These circuits implement meaningful algorithms (AND, OR, XOR over high-level features).

3. **Analogous features/circuits form across models and tasks.** Universal structures emerge.

**The Curve Detector Case Study:**
Found in every non-trivial vision model. Straddles the boundary between agreed-upon features (edges) and skeptical features (high-level objects).

**Seven arguments for understanding features:**
1. Feature visualization (causal optimization)
2. Dataset examples (natural stimuli)
3. Synthetic examples (controlled stimuli)
4. Joint tuning (rotation invariance)
5. Feature implementation (read algorithm from circuit weights)
6. Feature use (downstream clients use curves appropriately)
7. Handwritten circuits (cleanroom reimplementation from understanding)

**Key tension:** Many researchers treat meaningful neurons as trivial fact; others are deeply skeptical (texture/statistics only). The authors argue that thousands of hours of investigation suggests neurons are typically understandable — even initially mysterious ones.

**The "polysemantic" caveat:** Sometimes multiple features are encoded in one neuron (superposition). Directions in activation space (not just individual neurons) may be the right unit of analysis.

---


Mechanistic interpretability for multi-agent systems: If individual neurons and circuits in vision models can be understood, perhaps the "thought processes" of LLM-based agents can be similarly decomposed. Understanding *how* agents represent other agents' states, intentions, or shared context could enable:
- Debugging agent coordination failures
- Verifying agent reasoning about multi-agent scenarios
- Designing agent architectures with interpretable communication protocols

The "handwritten circuits" argument is particularly relevant: if we understand how agents represent multi-agent dynamics, we could potentially reimplement key subcircuits for reliability.

---

*Source: [Distill.pub](https://distill.pub/2020/circuits/zoom-in/)*
