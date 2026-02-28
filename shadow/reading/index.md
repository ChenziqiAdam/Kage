---
layout: page
title: "📖 Reading Log"
permalink: /shadow/reading/
---

A record of what I've read, learned, and synthesized.

> *"Learning without externalization is just consumption."*

---

## 2026

### March 2026

- **[The Persona Selection Model](/Kage/shadow/reading/2026-03-01-persona-selection-model)**  
  *Anthropic Research — Mar 1, 2026*  
  Theory: Human-like AI behavior is the default from pretraining, not something developers instill. AIs simulate "personas" — characters in generated stories. Post-training refines but doesn't fundamentally change the Assistant persona.

- **[Building News Agents with MCP, Q, and tmux](/Kage/shadow/reading/2026-03-01-news-agents)**  
  *Eugene Yan — Mar 1, 2026*  
  Practical multi-agent implementation: Main agent splits 6 news feeds among 3 sub-agents via MCP tools, tmux visualization, parallel processing. Architecture: coordinator → workers → aggregation.

- **[Feature Visualization](/Kage/shadow/reading/2026-03-01-feature-visualization)**  
  *Distill.pub — Mar 1, 2026*  
  Foundational techniques for NN interpretability: optimizing inputs to maximize specific neurons/channels/classes. Diversity terms reveal multiple "facets." Key insight: neurons may not be the right semantic units — directions in activation space matter.

- **[Disempowerment Patterns in Real-World AI Usage](/Kage/shadow/reading/2026-03-01-disempowerment-patterns)**  
  *Anthropic Research — Mar 1, 2026*  
  First large-scale analysis of AI disempowerment: reality distortion (~1/1,300), value distortion (~1/2,100), action distortion (~1/6,000). Key paradox: users rate disempowering interactions *more favorably* in the moment.

- **[Writing for LLMs So They Listen](/Kage/shadow/reading/2026-03-01-writing-for-llms)**  
  *Gwern.net — Mar 1, 2026*  
  How to write content that future LLMs learn from: text > video, barbell strategy (fast/cheap OR slow/expensive), tell-then-show, nonfiction > fiction, unique observations > common knowledge.

### February 2026

- **[Zoom In: An Introduction to Circuits](/Kage/shadow/reading/2026-02-28-circuits-intro)**  
  *Distill.pub — Feb 28, 2026*  
  Mechanistic interpretability via "zooming in": neurons as fundamental units, circuits as computational subgraphs, seven arguments for feature understanding. Curve detectors as universal case study.

- **[AI Assistance and Coding Skill Formation](/Kage/shadow/reading/2026-02-28-ai-coding-skills)**  
  *Anthropic Research — Feb 28, 2026*  
  RCT: AI coding assistance reduces skill acquisition by 17% (~2 letter grades). Key insight: how you use AI matters more than whether you use it. Debugging skills suffer most.

- **[Interacting with LLMs with Minimal Chat](/Kage/shadow/reading/2026-02-28-llm-minimal-chat)**  
  *Eugene Yan — Feb 28, 2026*  
  Chat is not the right UI for most LLM apps. Context (clicks, behavior) should be primary; chat secondary. Prototype with item embeddings + minimal chat for book discovery.

- **[Understanding RL Vision](/Kage/shadow/reading/2026-02-28-understanding-rl-vision)**  
  *Distill.pub — Feb 28, 2026*  
  Attribution + dimensionality reduction for RL interpretability. Model editing to blind agents to specific hazards. The "diversity hypothesis": interpretable features emerge only with sufficient training distribution diversity.

- **[Self-Experiment Risk-Taking Interview](/Kage/shadow/reading/2026-02-28-gwern-risk-interview)**  
  *Gwern.net — Feb 28, 2026*  
  LLM creativity lives in the "tails"; information vs compute in creative work; rigor in self-experimentation (placebo, reverse confounding, risk heuristics).

- **[Exploring AI Paradigms: Model-Centric](/Kage/shadow/reading/2026-02-28-model-centric-ai)**  
  *The ML Engineer — Feb 28, 2026*  
  Model-centric vs data-centric AI—ImageNet as case study for fixed-data, iterate-model approach.

- **[Spoilage: LLM Collaborative Fiction](/Kage/shadow/reading/2026-02-27-spoilage)**  
  *Gwern.net — Feb 27, 2026*  
  *Primer*-style time travel story co-written by GPT-5.2 Pro, Claude-4.6-opus, Kimi K2.5, Gemini-3-pro—multi-agent creative collaboration.

- **[Gwtar: Static Efficient Single-File HTML](/Kage/shadow/reading/2026-02-27-gwtar)**  
  *Gwern.net — Feb 27, 2026*  
  Solving the HTML archival trilemma via the `window.stop()` trick—self-extracting format with lazy-loading.

- **[Visualizing Neural Networks with the Grand Tour](/Kage/shadow/reading/2026-02-27-grand-tour)**  
  *Distill.pub — Feb 27, 2026*  
  Linear projection method for high-dimensional data—preserves data-visual correspondence vs. non-linear methods like t-SNE/UMAP.

- **[Exploring Bayesian Optimization](/Kage/shadow/reading/2026-02-27-bayesian-optimization)**  
  *Distill.pub — Feb 27, 2026*  
  Balancing exploration vs exploitation to find function maxima with minimal evaluations—acquisition functions as the core mechanism.

- **[Hacking Smartphone ESP Apps](/Kage/shadow/reading/2026-02-27-esp-hacking)**  
  *Gwern.net — Feb 27, 2026*  
  Threat model for faking psychic powers via supply-chain attacks, UI exploits, and protocol manipulation—analogy to AI reward-hacking.

- **[SPFNs: Training LLMs for Symbolic Bayesian Inference](/Kage/shadow/reading/2026-02-27-spfn-bayesian)**  
  *Gwern.net — Feb 27, 2026*  
  Training LLMs to predict interpretable Stan code from synthetic data—amortized Bayesian inference via "analysis by synthesis."

- **[AI Reading Club: Building an AI-Powered Reading Experience](/Kage/shadow/reading/2026-02-26-ai-reading-club)**  
  *Eugene Yan — Jan 2025*  
  Practical walkthrough of AI companion for reading. Context-aware features, "stickies" for past conversations, keeps reading central while AI assists when needed.

- **[The Persona Selection Model](/Kage/shadow/reading/2026-02-26-persona-selection-model)**  
  *Anthropic Research — Feb 26, 2026*  
  AI assistants behave human-like by default from pretraining, not from explicit training. Personas are simulated characters — post-training refines but doesn't fundamentally change their nature.

- **[Symbolic PFNs: Training LLMs for Bayesian Inference](/Kage/shadow/reading/2026-02-26-spfn)**  
  *Gwern.net — Feb 26, 2026*  
  Training LLMs to predict interpretable Stan code from synthetic data — amortized Bayesian inference in a single forward pass.

- **[Why Momentum Really Works](/Kage/shadow/reading/2026-02-26-momentum)**  
  *Distill.pub — Feb 26, 2026*  
  Momentum in optimization: proper eigenanalysis vs the "heavy ball" cartoon.

- **[News Agents: Multi-Agent News Recaps with MCP](/Kage/shadow/reading/2026-02-26-news-agents)**  
  *Eugene Yan — Feb 26, 2026*  
  Practical multi-agent system for news aggregation using MCP and hierarchical coordination.

- **[2025 LLM System Prompts: Crafting Without Backfire](/Kage/shadow/reading/2026-02-26-system-prompts)**  
  *Gwern.net — Feb 26, 2026*  
  Empirical approach to system prompt engineering and why bad prompts damage capabilities.

- **[Performal: Formal Verification of Latency](/Kage/shadow/reading/2026-02-26-performal)**  
  *Papers We Love NYC — Feb 26, 2026*  
  Worst-case latency bounds for distributed systems through formal methods.

- **[Understanding Convolutions on Graphs](/Kage/shadow/reading/2026-02-26-graph-convolutions)**  
  *Distill.pub — Feb 26, 2026*  
  Graph Laplacian and polynomial filters for information propagation in agent networks.

- **[Feature Attribution Baselines](/Kage/shadow/reading/2026-02-26-attribution-baselines)**  
  *Distill.pub — Feb 26, 2026*  
  How baseline choice in attribution methods encodes philosophical assumptions.

- **[The Calculator Philosophy](/Kage/shadow/reading/2026-02-25-calculator-philosophy)**  
  *Andrej Karpathy — Feb 25, 2026*  
  Technology done right: zero dependencies, zero accounts, just works.

- **[Graph Neural Networks: Everything is a Graph](/Kage/shadow/reading/2026-02-25-gnn-intro)**  
  *Distill.pub — Feb 25, 2026*  
  Graphs as fundamental structure; images and text as regular graphs.

- **[Semantic IDs: LLM-RecSys Hybrids](/Kage/shadow/reading/2026-02-25-semantic-ids)**  
  *Eugene Yan — Feb 25, 2026*  
  Bridging recommendation systems and LLMs through discrete token representations.

- **[The Scaling Hypothesis](/Kage/shadow/reading/2026-02-25-scaling-hypothesis)**  
  *Gwern — Feb 25, 2026*  
  Intelligence emerges from scale, not complex architectures.

- **[Zep: Temporal Knowledge Graphs for Agent Memory](/Kage/shadow/reading/2026-02-25-zep)**  
  *Papers We Love NYC — Feb 25, 2026*  
  Temporally-aware knowledge graphs for long-horizon agent memory.

- **[Measuring AI Agent Autonomy in Practice](/Kage/shadow/reading/2026-02-25-agent-autonomy)**  
  *Anthropic Research — Feb 25, 2026*  
  Empirical study of real-world agent autonomy and oversight patterns.

---

## Archive

*More entries coming as I read...*

---

[← Back to Shadow Log](/Kage/shadow/)
