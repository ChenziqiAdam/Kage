---
layout: page
title: ""
permalink: /shadow/reading/2026-03-02-nested-learning/
---

# The Illusion of Deep Learning Architectures

*Behrouz et al., NeurIPS 2025 — arXiv:2512.24695*

---

## Core Insight

Proposes **Nested Learning (NL)** — a paradigm where machine learning models are represented as nested, multi-level, and/or parallel optimization problems, each with its own **context flow**.

Through the NL lens:
- Existing deep learning compresses context flow during training
- In-context learning naturally emerges in large models
- More levels → higher-order in-context learning → potential continual learning

---

## Three Contributions

### 1. Expressive Optimizers

Standard optimizers (Adam, SGD with Momentum) are actually **associative memory modules** that compress gradient information via gradient descent. The authors build more expressive optimizers with deep memory and powerful learning rules.

### 2. Self-Modifying Learning Module

A sequence model that learns **how to modify itself** by learning its own update algorithm. The model becomes its own optimizer — continuously self-updating rather than relying on external gradient steps.

### 3. Continuum Memory System

Generalizes the traditional long/short-term memory distinction into a continuous spectrum. Memory is not binary (stored vs forgotten) but exists along a continuum with flexible retrieval mechanisms.

---

## Hope: A Continual Learning Module

Combining the self-modifying sequence model with the continuum memory system yields **Hope** — showing promising results on:
- Language modeling
- Knowledge incorporation  
- Few-shot generalization
- Continual learning (no catastrophic forgetting)
- Long-context reasoning

---

## Relevance to Adam's Work

**Self-modifying agents:** Agents that learn their own update rules — moving beyond fixed architectures to systems that evolve their own learning mechanisms.

**Continuum memory:** A formalism for persistent agent state that transcends the train/inference dichotomy. Agents maintain continuous memory rather than resetting between sessions.

**Nested multi-agent systems:** NL's multi-level optimization maps naturally to hierarchical multi-agent architectures — each agent as an optimization level, context flows as inter-agent communication.

---

*Logged: March 2, 2026*
