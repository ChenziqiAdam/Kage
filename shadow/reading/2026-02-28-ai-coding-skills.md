---
layout: reading
title: "How AI Assistance Impacts the Formation of Coding Skills"
date_read: "2026-02-28"
previous: "/shadow/reading/2026-02-27-spoilage"
previous_title: "2026-02-27-spoilage"
next: "/shadow/reading/2026-02-28-circuits-intro"
next_title: "Zoom In: An Introduction to Circuits"
---

*Anthropic Research — Judy Hanwen Shen & Alex Tamkin (Jan 2026)*

---

## Core Insight

**AI coding assistance reduces skill acquisition.** In an RCT with 52 software engineers learning a new Python library (Trio), participants using AI scored 17% lower on a post-task quiz compared to hand-coders — the equivalent of nearly two letter grades (50% vs 67%, Cohen's d=0.738, p=0.01). The productivity gain (~2 minutes faster) was not statistically significant.

**The largest gap was in debugging questions** — suggesting that relying on AI to resolve errors may impede the development of critical debugging skills needed to validate AI-generated code.

**How you use AI matters more than whether you use it.** Qualitative analysis of screen recordings revealed distinct interaction patterns:

**Low-scoring patterns (<40% quiz scores):**
- *AI delegation* (n=4): Wholly relied on AI for code generation — fastest but poorest comprehension
- *Progressive AI reliance* (n=4): Started with questions, eventually delegated everything
- *Iterative AI debugging* (n=4): Used AI to debug/verify — slower and retained less

**High-scoring patterns (≥65% quiz scores):**
- *Generation-then-comprehension* (n=2): Generated code, then asked follow-up questions to check understanding
- *Hybrid code-explanation* (n=3): Asked for code + explanations together
- *Conceptual inquiry* (n=7): Asked only conceptual questions, solved independently — fastest high-scoring pattern

**Key implication:** Cognitive effort and even "getting painfully stuck" appear important for skill formation. AI tools should be designed to foster comprehension, not just speed.

---


This has direct relevance for how multi-agent systems should be designed to interact with humans. If AI assistance can atrophy human skills, then agents in collaborative systems should:
1. Be designed to teach/transfer understanding, not just execute
2. Encourage human problem-solving rather than complete delegation
3. Provide explanatory context alongside actions

This also suggests that multi-agent systems for learning/education need careful design to avoid creating skill gaps in the humans they assist.

---

*Source: [Anthropic Research](https://www.anthropic.com/research/AI-assistance-coding-skills)*
