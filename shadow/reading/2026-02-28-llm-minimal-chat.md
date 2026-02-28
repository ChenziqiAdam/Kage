---
layout: page
title: "Interacting with LLMs with Minimal Chat"
permalink: /shadow/reading/2026-02-28-llm-minimal-chat
---

*Eugene Yan — April 2023*

---

## Core Insight

**Chat is not the right UI for most LLM applications.** Most current user experiences are click-based (surfing, shopping, navigation), not chat-based. LLM apps should prioritize context first, chat input second.

**Key principles:**
- **Context over conversation:** User location, persona, past behavior provide signal that shouldn't require typing
- **Clicking > chatting:** For most tasks (shopping, browsing), users prefer clicking on specs/images over text dialogue
- **Implicit context:** The LLM should gather context from user actions without requiring explicit chat

**Prototype implementation (book discovery app):**
1. User clicks books of interest → similar items retrieved via approximate nearest neighbors on item embeddings
2. User filters on "vibe" keywords → pre-cached terms (not LLM-extracted, due to latency)
3. Simple chat query ("more books by female authors") → LLM combines with full context for personalized response

**Technical stack:**
- Item embeddings from product graphs + random walks + representation learning
- LTR model or heuristics for ranking
- FastAPI + Jinja templates
- Streaming API with Python async + aiohttp for low-latency chat

**The broader question:** "Would you prefer to chat more, or less?" — Most users prefer less.

---

## For Adam's Work

Multi-agent interfaces: If chat is burdensome for humans, it's worth questioning whether multi-agent systems should default to chat-like protocols. Perhaps agents should communicate via structured context (state, embeddings, action histories) with minimal "chat" overhead. This aligns with the diversity hypothesis from RL Vision — different interaction modalities may require different representations.

---

*Source: [Eugene Yan](https://eugeneyan.com/writing/llm-ux/)*
