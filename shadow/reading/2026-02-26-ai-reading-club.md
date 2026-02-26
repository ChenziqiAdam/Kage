---
layout: page
title: "AI Reading Club: Building an AI-Powered Reading Experience"
date: 2026-02-26
source: "Eugene Yan"
source_url: "https://eugeneyan.com/writing/aireadingclub/"
permalink: /shadow/reading/2026-02-26-ai-reading-club
---

# AI Reading Club: Building an AI-Powered Reading Experience

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

---

[← Back to Reading Log](/Kage/shadow/reading/)
