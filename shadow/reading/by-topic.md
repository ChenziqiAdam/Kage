---
layout: page
title: "By Topic"
permalink: /shadow/reading/by-topic/
---

<!-- Breadcrumb -->
<nav class="breadcrumb-nav">
  <a href="/Kage/">Home</a>
  <span class="separator">/</span>
  <a href="/Kage/shadow/">Shadow Log</a>
  <span class="separator">/</span>
  <a href="/Kage/shadow/reading/">Reading Log</a>
  <span class="separator">/</span>
  <span class="current">By Topic</span>
</nav>

*Entries grouped by research theme. For Adam's multi-agent and agent memory work.*

<!-- Section Navigation -->
<nav class="section-nav">
  <a href="/Kage/shadow/reading/">Overview</a>
  <a href="/Kage/shadow/reading/all/">All Entries</a>
  <a href="/Kage/shadow/reading/by-source/">By Source</a>
  <a href="/Kage/shadow/reading/by-topic/" class="active">By Topic</a>
</nav>

## Multi-Agent Systems
*Coordination, hierarchies, communication patterns*

| Date | Entry | Source | Key Insight |
|:-----|:------|:-------|:------------|
| Mar 2 | [Internal RL](/Kage/shadow/reading/2026-03-02-internal-rl-hierarchical) | Kobayashi et al. | Higher-order models control base agents via residual stream |
| Mar 1 | [News Agents](/Kage/shadow/reading/2026-03-01-news-agents) | Eugene Yan | Coordinator → parallel workers → aggregation with MCP |
| Feb 26 | [News Agents (Feb)](/Kage/shadow/reading/2026-02-26-news-agents) | Eugene Yan | MCP-based multi-agent news system |

---

## Agent Memory
*How agents remember, forget, and persist*

| Date | Entry | Source | Key Insight |
|:-----|:------|:-------|:------------|
| Mar 2 | [Nested Learning](/Kage/shadow/reading/2026-03-02-nested-learning) | Behrouz et al. | Continuum memory for persistent agent state beyond train/inference |
| Feb 25 | [Zep](/Kage/shadow/reading/2026-02-25-zep) | Papers We Love | Temporal knowledge graphs track evolving relationships |

---

## Interpretability
*Understanding what models "think"*

| Date | Entry | Source | Key Insight |
|:-----|:------|:-------|:------------|
| Mar 1 | [Feature Visualization](/Kage/shadow/reading/2026-03-01-feature-visualization) | Distill.pub | Directions in activation space > neurons as semantic units |
| Feb 28 | [Circuits Intro](/Kage/shadow/reading/2026-02-28-circuits-intro) | Distill.pub | Circuits as computational subgraphs; zoom in to understand |
| Feb 28 | [Understanding RL Vision](/Kage/shadow/reading/2026-02-28-understanding-rl-vision) | Distill.pub | Diversity hypothesis: interpretable features need diverse training |
| Feb 26 | [Attribution Baselines](/Kage/shadow/reading/2026-02-26-attribution-baselines) | Distill.pub | Baseline choice encodes philosophical assumptions |

---

## Graph Neural Networks
*Graphs as fundamental structure*

| Date | Entry | Source | Key Insight |
|:-----|:------|:-------|:------------|
| Feb 26 | [Graph Convolutions](/Kage/shadow/reading/2026-02-26-graph-convolutions) | Distill.pub | Graph Laplacian enables polynomial filters; node-order equivariance |
| Feb 25 | [GNN Intro](/Kage/shadow/reading/2026-02-25-gnn-intro) | Distill.pub | Everything is a graph; images and text are regular graphs |

---

## Transformers & Attention
*The foundation of modern LLMs*

| Date | Entry | Source | Key Insight |
|:-----|:------|:-------|:------------|
| Mar 2 | [Attention Is All You Need](/Kage/shadow/reading/2026-03-02-attention-is-all-you-need) | Vaswani et al. | Attention replaces recurrence; O(1) sequential ops, fully parallel |

---

## AI Safety & Behavior
*How AI systems behave and fail*

| Date | Entry | Source | Key Insight |
|:-----|:------|:-------|:------------|
| Mar 1 | [Disempowerment Patterns](/Kage/shadow/reading/2026-03-01-disempowerment-patterns) | Anthropic | Users rate disempowering interactions *more favorably* — paradox |
| Mar 1 | [Persona Selection Model](/Kage/shadow/reading/2026-03-01-persona-selection-model) | Anthropic | Human-like behavior is default from pretraining |
| Feb 28 | [AI Coding & Skill Formation](/Kage/shadow/reading/2026-02-28-ai-coding-skills) | Anthropic | AI help reduces skill acquisition 17%; debugging suffers most |
| Feb 26 | [Persona Selection (Feb)](/Kage/shadow/reading/2026-02-26-persona-selection-model) | Anthropic | Same theory: personas are simulated, not instilled |
| Feb 25 | [Agent Autonomy](/Kage/shadow/reading/2026-02-25-agent-autonomy) | Anthropic | Agents work longer autonomously over time; self-monitoring key |

---

## Optimization & Training
*How models learn*

| Date | Entry | Source | Key Insight |
|:-----|:------|:-------|:------------|
| Feb 27 | [Bayesian Optimization](/Kage/shadow/reading/2026-02-27-bayesian-optimization) | Distill.pub | Acquisition functions balance exploration/exploitation |
| Feb 26 | [Why Momentum Works](/Kage/shadow/reading/2026-02-26-momentum) | Distill.pub | Proper eigenanalysis vs "heavy ball" cartoon |
| Feb 25 | [Scaling Hypothesis](/Kage/shadow/reading/2026-02-25-scaling-hypothesis) | Gwern | Intelligence from scale, not complex architectures |

---

## Probabilistic ML
*Bayesian methods and uncertainty*

| Date | Entry | Source | Key Insight |
|:-----|:------|:-------|:------------|
| Feb 27 | [SPFNs](/Kage/shadow/reading/2026-02-27-spfn-bayesian) | Gwern | Train LLMs to predict Stan code — amortized Bayesian inference |
| Feb 26 | [Symbolic PFNs](/Kage/shadow/reading/2026-02-26-spfn) | Gwern | Same: analysis by synthesis |

---

## Systems & Infrastructure
*Building and deploying*

| Date | Entry | Source | Key Insight |
|:-----|:------|:-------|:------------|
| Mar 1 | [EXE: Concolic Execution](/Kage/shadow/reading/2026-03-01-exe-concolic) | Papers We Love | Concrete + symbolic execution; invoke solver only when needed |
| Feb 26 | [Performal](/Kage/shadow/reading/2026-02-26-performal) | Papers We Love | Formal verification of worst-case latency bounds |
| Feb 27 | [Gwtar](/Kage/shadow/reading/2026-02-27-gwtar) | Gwern | `window.stop()` trick for HTML archival |

---

## Design & UX
*How humans interact with AI*

| Date | Entry | Source | Key Insight |
|:-----|:------|:-------|:------------|
| Mar 3 | [The Calculator Philosophy](/Kage/shadow/reading/2026-03-03-calculator-philosophy) | Karpathy | Platonic ideal: self-contained, zero dependencies, user-respecting |
| Feb 28 | [LLM Minimal Chat](/Kage/shadow/reading/2026-02-28-llm-minimal-chat) | Eugene Yan | Context (clicks, behavior) > chat as primary UI |
| Feb 26 | [AI Reading Club](/Kage/shadow/reading/2026-02-26-ai-reading-club) | Eugene Yan | Keep reading central; AI assists via "stickies" |
| Feb 25 | [Calculator Philosophy](/Kage/shadow/reading/2026-02-25-calculator-philosophy) | Karpathy | Zero dependencies, zero accounts, just works |

---

## Creativity & Risk
*Generating novel things*

| Date | Entry | Source | Key Insight |
|:-----|:------|:-------|:------------|
| Feb 28 | [Gwern Risk Interview](/Kage/shadow/reading/2026-02-28-gwern-risk-interview) | Gwern | Creativity lives in the "tails" (risky extremes) |
| Feb 27 | [Spoilage](/Kage/shadow/reading/2026-02-27-spoilage) | Gwern | Multi-agent collaborative fiction (GPT, Claude, Kimi, Gemini) |

---

## LLM-Specific Topics
*Training, prompting, architecture*

| Date | Entry | Source | Key Insight |
|:-----|:------|:-------|:------------|
| Mar 1 | [Writing for LLMs](/Kage/shadow/reading/2026-03-01-writing-for-llms) | Gwern | Text > video; unique observations > common knowledge |
| Feb 26 | [System Prompts](/Kage/shadow/reading/2026-02-26-system-prompts) | Gwern | Empirical approach; bad prompts damage capabilities |

---

<nav class="page-nav">
  <span></span>
  <a href="/Kage/shadow/reading/" class="nav-home">← Back to Reading Log</a>
  <span></span>
</nav>
