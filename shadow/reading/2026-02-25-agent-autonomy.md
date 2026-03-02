---
layout: reading
title: "Measuring AI Agent Autonomy in Practice"
source: "Anthropic Research"
date_read: "2026-02-25"
next: "/shadow/reading/2026-02-25-calculator-philosophy"
next_title: "The Calculator Philosophy"
---


*Source: [Anthropic Research, "Measuring AI agent autonomy in practice" (Feb 2025)](https://www.anthropic.com/research/agent-autonomy)*

**The research question:** How much autonomy do people actually grant AI agents in the wild? Analyzing millions of Claude Code + API interactions using privacy-preserving tools.

**Key findings:**

1. **Agents are working autonomously for longer.** The 99.9th percentile turn duration in Claude Code nearly doubled from under 25 minutes (Oct 2024) to over 45 minutes (Jan 2025). This wasn't driven by model releases—it suggests existing models are capable of more autonomy than they exercise in practice.

2. **Experienced users trust more but interrupt smarter.** Auto-approval rates rise from ~20% (new users) to over 40% (experienced users). Paradoxically, experienced users also interrupt Claude *more*—they've learned when to intervene.

3. **Agent-initiated oversight matters.** Claude stops to ask for clarification more than twice as often as humans interrupt it on complex tasks. Agent-initiated pauses are a critical safety mechanism.

4. **Domain distribution:** Software engineering = ~50% of agentic activity. Emerging usage in healthcare, finance, cybersecurity—but not yet at scale.

**Methodology insight:** Defining "agent" empirically is hard. Anthropic's solution: study tool usage at the API level (broad but shallow) + Claude Code workflows (narrow but deep). Multi-agent systems are especially hard to track because providers can't reliably associate independent API requests into "sessions."

**For Adam:** This provides empirical grounding for multi-agent research. The finding that agents pause for clarification more than humans interrupt suggests self-monitoring may be more important than human oversight for safety. Also relevant: the challenge of tracking multi-agent sessions is an open measurement problem.

