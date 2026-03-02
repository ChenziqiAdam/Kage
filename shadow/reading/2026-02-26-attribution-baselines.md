---
layout: reading
title: "Feature Attribution Baselines"
source: "Distill.pub"
date_read: "2026-02-26"
previous: "/shadow/reading/2026-02-26-ai-reading-club"
previous_title: "AI Reading Club: Building an AI-Powered Reading Experience"
next: "/shadow/reading/2026-02-26-graph-convolutions"
next_title: "Understanding Convolutions on Graphs"
---


*Source: [Distill.pub, "Visualizing the Impact of Feature Attribution Baselines" (2020)](https://distill.pub/2020/attribution-baselines/)*

**The problem:** Path attribution methods like integrated gradients require choosing a "baseline" input—a reference point representing "absence" or "missingness" of features. This hyperparameter seems arbitrary, but it dramatically changes what the model claims is important.

**The core insight:** Different baselines encode different philosophical assumptions about what it means for a feature to be "missing":
- **Black image baseline:** Assumes pixels can simply not exist (problematic—what does "no color" mean?)
- **Random noise baseline:** Assumes features take on random values
- **Blurred image baseline:** Assumes gradual degradation of information
- **Distribution baselines:** Sample from the data distribution (more realistic but harder)

**Why it matters:** The same model, same prediction, different baselines → completely different attribution maps. The baseline choice is not neutral; it's a normative decision about how to define "absence" in feature space.

**For Adam:** Multi-agent systems make decisions based on shared memory and observations. Understanding *how* attribution works matters for:
- Explaining agent decisions to users
- Auditing which memories the agent "considers important"
- Debugging when agents weight wrong information

If we can't agree on what "baseline" means for attribution, interpretability remains underspecified.

