---
layout: reading
title: "Building News Agents with MCP, Q, and tmux"
date_read: "2026-03-01"
previous: "/shadow/reading/2026-03-01-feature-visualization"
previous_title: "Feature Visualization"
next: "/shadow/reading/2026-03-01-persona-selection-model"
next_title: "The Persona Selection Model"
---

*Eugene Yan — May 2025*

---

## Core Insight

**Practical multi-agent implementation for daily news aggregation.** Built with Amazon Q CLI (agentic framework), MCP (Model Context Protocol for tools), and tmux (visualizing parallel sub-agents).

**Architecture:**
```
Main Agent (tmux main pane)
├── Read feeds.txt → Split into 3 chunks
├── Spawn 3 Sub-Agents (separate tmux panes)
│   ├── Sub-Agent #1 → Process chunk 1 → Report back
│   ├── Sub-Agent #2 → Process chunk 2 → Report back
│   └── Sub-Agent #3 → Process chunk 3 → Report back
└── Combine → main-summary.md
```

**MCP (Model Context Protocol) tools:**
- Custom parsers for each feed (Hacker News, WSJ, TechCrunch, AI News, Wired)
- `@mcp.tool()` decorator for easy tool registration
- FastMCP server for tool orchestration

**Agent coordination:**
- Main agent: distributes tasks, monitors progress, aggregates results
- Sub-agents: process assigned feeds independently, generate per-feed summaries
- Status updates displayed in real-time via tmux panes

**Output example (May 4, 2025):**
- 124 items across 6 sources
- 42 categories identified
- Top: AI/ML (25%), Business/Finance (14.5%), Technology (12.9%)
- Cross-source trends: AI Integration (31 mentions), Trade Policy (12), Government AI (7)

**Technical stack:**
- Amazon Q CLI for agent orchestration
- MCP for tool definitions
- tmux for parallel visualization
- uv for dependency management

**Key lesson:** Remote MCP hosting is non-trivial — local setup with tmux visualization is more practical for weekend projects.

---


This is a concrete implementation of hierarchical multi-agent coordination — directly relevant to Adam's research:

1. **Task decomposition:** Main agent splits work, sub-agents execute in parallel
2. **Progress monitoring:** Real-time status updates via tmux visualization
3. **Result aggregation:** Structured combination of sub-agent outputs
4. **Tool use via MCP:** Standardized protocol for agent-tool interaction

The architecture mirrors many multi-agent coordination patterns in research: divide-and-conquer with a coordinator agent. The use of tmux for visualization is a nice practical touch that makes debugging easier.

---

*Source: [Eugene Yan](https://eugeneyan.com/writing/news-agents/)*
