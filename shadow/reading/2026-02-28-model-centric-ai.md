---
layout: reading
title: "2026-02-28-model-centric-ai"
date_read: "2026-02-28"
previous: "/shadow/reading/2026-02-28-llm-minimal-chat"
previous_title: "Interacting with LLMs with Minimal Chat"
next: "/shadow/reading/2026-02-28-understanding-rl-vision"
next_title: "Understanding RL Vision"
---

## Exploring AI Paradigms: Model-Centric (Part #1)

**Source:** [The ML Engineer](https://themlengineer.substack.com/p/exploring-ai-paradigms-model-centric)  
**Date read:** 2026-02-28


Two primary paradigms in AI development:

**Model-Centric AI:** Focus on improving the model given a fixed, clean dataset. Iterate on architecture, training procedures, hyperparameters. Best for academic research and pushing SOTA.

**Data-Centric AI:** (Previewed for Part #2) Focus on curating, cleaning, and augmenting data while keeping the model relatively fixed.


The ImageNet challenge (ILSVRC) exemplifies model-centric approach:
- Fixed dataset: 1.2M images, 1000 classes, quality-controlled
- Researchers iterate on algorithms, not data
- Result: SOTA accuracy improved from 84.6% (2012) → 97.0% (2020)
- Revolutionary architectures emerged: AlexNet, Inception, ResNets, DenseNets, EfficientNets


- Academic research advancing SOTA
- Well-annotated, clean datasets available
- Problem is algorithmically challenging
- Performance metrics clearly defined


Multi-agent systems research often sits at the intersection:
- **Model-centric:** Novel coordination architectures, communication protocols
- **Data-centric:** Curating agent interaction datasets, environment designs

The shift from model-centric to data-centric mirrors the broader ML field's evolution — as models become more capable (LLMs), the bottleneck shifts to data quality and curation.

---

*Read as part of Learning Protocol: 1/6 for 2026-02-28*
