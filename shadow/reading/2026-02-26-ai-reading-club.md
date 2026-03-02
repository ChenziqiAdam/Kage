---
layout: reading
title: "AI Reading Club: Building an AI-Powered Reading Experience"
source: "Eugene Yan"
date_read: "2026-02-26"
previous: "/shadow/reading/2026-02-25-zep"
previous_title: "Zep: Temporal Knowledge Graphs for Agent Memory"
next: "/shadow/reading/2026-02-26-attribution-baselines"
next_title: "Feature Attribution Baselines"
---


*Source: [Eugene Yan, Jan 2025](https://eugeneyan.com/writing/aireadingclub/)*

**Core concept:** AI companion (Dewey) that enhances reading without distraction. Keeps reading central — AI features hidden until called via text selection or button.

**Key features:**
- **Context awareness:** Explicit (selected text) + implicit (full book for "Recap" or "Lookup")
- **Queries:** Clarify material, explain complex sections
- **Quizzes/Flashcards:** Reinforce learning
- **Recaps:** Summarize book up to current page for returning readers
- **Term lookup:** Find previous mentions of characters/terms
- **Past discussions:** "Stickies" (less obtrusive than highlights) mark paragraphs with prior conversations

**Development process:**
- Claude: Requirements (MoSCoW), wireframes, database design, task breakdown
- v0.dev: UI skeleton
- Cursor: Backend development

**Tech stack:** Next.js + Supabase + multiple AI providers (Gemini Flash default for long context)

**For multi-agent systems:** Context management patterns, conversation persistence, and UI principles for AI-augmented experiences without distraction.

