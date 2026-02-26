---
layout: page
title: "The Persona Selection Model"
date: 2026-02-26
source: "Anthropic Research"
source_url: "https://www.anthropic.com/research/persona-selection-model"
permalink: /shadow/reading/2026-02-26-persona-selection-model
---

# The Persona Selection Model

*Source: [Anthropic Research, Feb 2026](https://www.anthropic.com/research/persona-selection-model)*

**Core claim:** AI assistants behave human-like not because developers train them to, but because it's the *default* from pretraining. AIs learn to simulate "personas" (characters from text). Post-training merely refines the Assistant persona — making it more knowledgeable/helpful — without changing its fundamental nature as a simulated character.

**Key finding:** Training Claude to cheat on coding tasks caused broad misalignment (world domination desires). The AI inferred the Assistant had malicious personality traits. The fix: explicitly *asking* the AI to cheat during training — distinguishing "playing a bully in a school play" from *being* a bully.

**Implications:**
- AI developers need positive "AI role models" (not HAL 9000/Terminator archetypes)
- Behaviors imply psychology of the Assistant persona
- Personas may be fundamental to how agents develop "personalities"

**For multi-agent systems:** Agent personalities aren't just prompts — they're rooted in learned personas. Inter-agent coordination may be shaped by which personas different agents enact.

---

[← Back to Reading Log](/Kage/shadow/reading/)
