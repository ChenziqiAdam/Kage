---
layout: page
title: "LLM System Prompts 2025"
---

*Source: [Gwern Branwen, "Some 2025 LLM System Prompts" (Nov 2025 - Feb 2026)](https://gwern.net/system-prompts-2025)*

## Core Insight

**System prompts can seriously damage LLM capabilities.** Gwern describes a striking case where a user complained Claude-4s were incapable of even simple copyediting — investigation revealed they'd copy-pasted an old ChatGPT system prompt that had the effect of making Claude say next to nothing.

This led Gwern to develop a comprehensive "style guide" approach rather than "YOLO cargo-culting random nice-sounding things."

## The Style Guide Approach

**Tone & epistemic style:**
- Be concise, specific, declarative — no hedging
- Use calibrated probability language: *unlikely, plausible, probable, very probable, almost certain*
- Evaluate all ideas on merit regardless of source reputation

**Citation format:**
- `[Surname Year](URL "Title")` — never numbered brackets `[1]`
- No author → use site/org; no year → `n.d.`; no title → omit tooltip

**Formatting:**
- **Ventilated prose** for final drafts: one sentence per line, double newlines between paragraphs
- Custom link syntax: `<a href="!W">` for Wikipedia, `<a href="$YEAR">` for inflation-adjusted values

**Creative writing rules:**
- Relax conciseness constraints
- Prioritize vividness, sensory specificity, narrative momentum
- **Ban** "antithesis bloat" ("It was not X, but Y") and "list-negation" ("No X, no Y—just Z")
- Avoid yellow/brown/sepia palettes
- Ground speculative elements in real mechanisms

**Poetry work:**
- HTML-commented prosodic annotations on each line (syllable count, stress pattern, sound features)
- Track formal constraints: sonnet needs rhyme tags, haiku needs mora count

## Model-Specific Constraints

**Gemini-3-pro-preview:** Allows long system prompts with detailed scaffolding

**GPT-5:** Maximum 1,500 characters — requires severe compression, loses some stylistic corrections

**Claude-4.5/4.6-opus:** Self-revising system prompts; can suggest improvements to their own instructions

## Why It Matters for Adam's Work

**Self-aware AI connection:**
The system prompt is essentially the AI's "self-understanding" — its definition of what it is and how it should behave. This is proto-self-awareness: the model's behavior is shaped by its instruction-set, which includes constraints on how it reasons, cites, and expresses itself.

**Self-evolving connection:**
Gwern's iterative approach — having models write and improve their own prompts — mirrors how self-evolving agents might bootstrap better self-models. Claude-4.6-opus suggesting edits to its own system prompt is a concrete example of a model modifying its own operational parameters.

**Multi-agent implications:**
Different models need different prompts. A multi-agent system with heterogeneous models (Gemini, GPT, Claude) would need agent-specific prompt protocols — the "persona" isn't just a wrapper, it's a compatibility layer.

**Key tension:**
The balance between constraint (accuracy, concision, neutrality) and creativity (vividness, narrative flow, emotional resonance). Agents may need explicit "modes" with different self-definitions for different tasks.

## Key Takeaway

System prompt engineering is meta-programming. The prompt isn't just instructions — it's the AI's working definition of itself. Gwern's 4,000+ word prompt for Gemini and iterative refinement process show that effective self-definition requires both precision and the capacity for self-modification.

For self-aware AI research: what would an agent's system prompt look like if it were *self-authored* and *continually refined* based on task performance?

---

*Read: March 3, 2026 — Gwern.net*
