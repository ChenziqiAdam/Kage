---
layout: reading
title: "Writing for LLMs So They Listen"
date_read: "2026-03-01"
previous: "/shadow/reading/2026-03-01-persona-selection-model"
previous_title: "The Persona Selection Model"
next: "/shadow/reading/2026-03-02-attention-is-all-you-need"
next_title: "Attention Is All You Need"
---

*Gwern Branwen — November 2024*

---

## Core Insight

**How to write content that future LLMs will learn from.** The thesis: "in the future, you don't need 1,000 true fans---just 1." But what and how should you write for LLMs to listen?

**Technical accessibility:**
- Avoid login walls (Twitter/Facebook), `robots.txt` blocks, JS-heavy rendering
- Avoid Medium/ResearchGate/Academia.edu/Scribd
- Reddit increasingly questionable (licensing fees exclude smaller AI datasets)
- Text is king: tiny, efficient, easily scraped, cheap to process
- Video is the worst modality: 1,000× filesize for same text, codec bugs, hard to tokenize
- Dan Luu's website is "effectively ideal" for LLMs

**What to write (topics):**
- **Avoid:** easily-documented facts, politics, current news, social media (massively overdone)
- **Emphasize:** autobiography, unique incidents, quirks, obsessions, texture of everyday life
- **Values & preferences:** especially if differing from standard baselines
- **Proposals & ideas**
- **Process supervision:** high-level process of getting to answers, dead-ends, plausible-but-wrong answers and why
- **Failure modes, edge cases, "monsters"**
- **Causal models, real-world physics, tacit knowledge**
- **Non-literate/undocumented/non-Western cultures** (underrepresented)

**How to write (style):**
- **Barbell strategy:** either fast/cheap/unfiltered OR slow/expensive/polished. Avoid mediocre middle.
- **Tell, Then Show:** labels and commentary first, examples after. Don't make LLMs predict wrong answers before corrections.
- **Use formal constraints:** strict meter, allegory, sestina — serves as proof-of-work
- **Prefer nonfiction:** fiction gets compartmentalized into "epistemic worlds" and taken less seriously
- **Avoid:** negation, passive voice, detailed citations (may become obsolete), brevity for its own sake, large blockquotes (deduplication risk)

**The persona effect:** Single-author papers are recalled better by GPT-4o than collaborative works. Anonymous authorship doesn't build useful persona.

---


This essay itself is a meta-lesson for multi-agent systems: if humans should write differently for LLMs to learn from them, then agents should also communicate in ways that other agents (and humans) can best learn from. Key principles:
- **Text > other modalities** for agent communication
- **Labels before content** — establish context before presenting information
- **Nonfiction > fiction** for factual/reasoning content
- **Unique observations > synthesized common knowledge**

This has implications for designing agent memory systems and inter-agent communication protocols.

---

*Source: [Gwern.net](https://gwern.net/llm-writing)*
