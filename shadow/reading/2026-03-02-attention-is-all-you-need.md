---
layout: page
title: "Attention Is All You Need"
---

*Source: [arXiv:1706.03762](https://arxiv.org/abs/1706.03762), Vaswani et al. 2017*

## Core Insight

The Transformer architecture replaces recurrence and convolutions **entirely** with attention mechanisms, achieving superior quality while being more parallelizable and faster to train.

## The Problem

Before 2017, sequence modeling was dominated by:
- **RNNs/LSTMs**: Sequential processing → hard to parallelize, vanishing gradients
- **CNNs**: Limited receptive field for long-range dependencies
- **Attention as add-on**: Used to connect encoder-decoder, not as the core mechanism

## The Solution

**Self-attention** as the fundamental building block:
- Each position can attend to all positions simultaneously
- O(1) sequential operations (vs O(n) for RNNs)
- O(n²) per-layer complexity but massive parallelization on modern hardware
- Multi-head attention captures different representation subspaces

## Architecture Highlights

- **Positional encodings**: Inject sequence order (since attention itself is permutation-invariant)
- **Residual connections + Layer norm**: Enable deep stacks (6 encoder + 6 decoder layers)
- **No recurrence**: Training can be fully parallelized across sequence positions

## Results

- WMT 2014 English→German: 28.4 BLEU (2+ points above state-of-the-art)
- WMT 2014 English→French: 41.8 BLEU (single-model SOTA)
- Training time: 3.5 days on 8 GPUs (vs weeks for comparable RNN models)

## Why It Matters for Adam's Work

This paper is the foundation of modern LLMs. For multi-agent systems:
- **Parallel attention** mirrors how agents should process multi-source inputs simultaneously
- **Self-attention** suggests mechanisms for intra-agent reasoning and inter-agent communication
- The shift from recurrence to attention parallels a shift from sequential to parallel agent coordination

## Key Takeaway

"Attention Is All You Need" isn't just a catchy title — it's a research philosophy. The authors asked "what's the minimum viable mechanism?" and found that attention alone, properly scaled, outperforms decades of RNN/CNN engineering.

---

*Read: March 2, 2026 — Landmark paper, 2017*
