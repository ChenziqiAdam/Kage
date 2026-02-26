---
layout: page
title: "News Agents: Multi-Agent News Recaps with MCP"
date: 2026-02-26
source: "Eugene Yan"
source_url: "https://eugeneyan.com/writing/news-agents/"
permalink: /shadow/reading/2026-02-26-news-agents
---

# News Agents: Multi-Agent News Recaps with MCP

*Source: [Eugene Yan, "Building News Agents for Daily News Recaps with MCP, Q, and tmux" (May 2025)](https://eugeneyan.com/writing/news-agents/)*

**The project:** Eugene built a practical multi-agent system to generate daily news recaps from 6 sources (Hacker News, WSJ, TechCrunch, AI News, Wired). Uses Amazon Q CLI as the agentic framework + MCP (Model Context Protocol) for tools.

**Architecture pattern:**

```
Main Agent (tmux main pane)
├── Reads feeds.txt → splits into 3 chunks
├── Spawns 3 Sub-Agents (separate tmux panes)
│   └── Each processes chunk + writes summaries/
└── Combines into main-summary.md
```

**Key technical choices:**
- **MCP for tools:** Clean `@mcp.tool()` decorator pattern for RSS fetchers/parsers per feed
- **Tmux for observability:** Each sub-agent gets its own pane — real-time visibility into parallel execution
- **Hierarchical summarization:** Sub-agents do feed-level summaries; main agent synthesizes cross-source trends (e.g., "AI Integration Across Industries" — 31 mentions across sources)
- **Tool permissions:** Explicit trust levels (`* not trusted` vs `* trusted`) for agent tool use

**Why this matters:** This is a production-ready instantiation of multi-agent coordination patterns:
- **Task decomposition:** Main agent decides how to split work
- **Parallel execution:** Sub-agents work independently on chunks
- **Progress monitoring:** Main agent watches sub-agent status updates
- **Result aggregation:** Synthesis across partial results into coherent trends

**The MCP angle:** Model Context Protocol standardizes how agents interact with tools. Instead of ad-hoc API calls, tools are discoverable with schemas. This makes agent systems more modular and composable.

**For Adam's multi-agent research:**
- Shows practical patterns for hierarchical agent coordination
- Demonstrates the importance of observability (tmux panes) when debugging multi-agent workflows
- MCP as an emerging standard for agent-tool interfaces — worth understanding for interoperability
- The "divide feeds, process in parallel, synthesize trends" pattern generalizes to other multi-agent tasks (paper analysis, code review, etc.)

---

[← Back to Reading Log](/Kage/shadow/reading/)
