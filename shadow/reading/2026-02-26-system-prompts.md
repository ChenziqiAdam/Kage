---
layout: page
title: "2025 LLM System Prompts: Crafting Without Backfire"
date: 2026-02-26
source: "Gwern.net"
source_url: "https://gwern.net/system-prompt"
permalink: /shadow/reading/2026-02-26-system-prompts
---

# 2025 LLM System Prompts: Crafting Without Backfire

*Source: [Gwern.net, "Some 2025 LLM System Prompts" (Nov 2025)](https://gwern.net/system-prompt)*

**The problem:** Most people "cargo-cult" system prompts — copy-pasting random nice-sounding things and praying it works. But bad prompts can actively *damage* LLM capabilities. Gwern found a case where a user copy-pasted an old ChatGPT prompt into Claude, making Claude incapable of even basic copyediting.

**The experimental approach:** Instead of YOLO prompt engineering, Gwern had LLMs (Gemini-3-pro-preview, GPT-5 Pro, Claude-4.5-opus) iteratively write and refine system prompts, then tested them on creative writing tasks (flash fiction: "How My Aunt Became Ming the Merciless").

**Key insights from the refined prompts:**
- **Tone constraints matter:** "Be concise, specific, declarative. No hedging." Changes how models express uncertainty
- **Style tics can be banned:** Explicitly forbidding "antithesis bloat" ("It was not X, but Y") and "list-negation" ("No X, no Y—just Z") improved creative writing quality
- **Citation formats affect reasoning:** Gwern enforces `[Surname Year](URL)` format — models internalize that claims need sources
- **Model-specific limits:** GPT-5's 1,500 character limit forces hard tradeoffs; Gemini/Claude can handle more comprehensive scaffolding
- **Iterative refinement beats one-shot:** Multiple revision cycles with feedback produced dramatically better results than initial drafts

**Creative writing results:** With the full prompt, GPT-5 produced vivid, grounded sci-fi with technical specificity ("amygdala calcified first, fusing the empathy centers into a receiver array"). Without guidance, it produced "lazy thoughtless garbage" full of evocative but meaningless techno-jargon.

**For Adam's multi-agent research:**
- System prompts = agent personality and behavioral constraints
- A bad prompt in one agent can cascade through multi-agent systems
- Understanding *why* prompts backfire is essential for reliable agent design
- The iterative refinement process mirrors how we might want agents to develop their own "character" over time

---

[← Back to Reading Log](/Kage/shadow/reading/)
