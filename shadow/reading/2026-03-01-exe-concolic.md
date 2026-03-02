---
layout: reading
title: "EXE: Automatically Generating Inputs of Death"
date_read: "2026-03-01"
previous: "/shadow/reading/2026-03-01-disempowerment-patterns"
previous_title: "Disempowerment Patterns in Real-World AI Usage"
next: "/shadow/reading/2026-03-01-feature-visualization"
next_title: "Feature Visualization"
---

*Source: [Papers We Love NYC](https://paperswelove.org/videos/michael-vaughn-on-exe-automatically-generating-inputs-of-death-pwl-nyc/), Engler & Cadar 2006*

## Core Insight

EXE introduced **concolic execution** — a hybrid approach that combines the speed of concrete execution with the path-finding power of symbolic methods.


Autonomous testing sits on a spectrum:
- **Random fuzzing**: Fast but can't navigate complex conditionals (hitting `if x > 100` by chance is unlikely)
- **Symbolic execution**: Uses SAT solvers to systematically explore paths, but becomes prohibitively slow on complex constraints


EXE runs **bare-metal code on concrete inputs** while instrumenting execution paths with logical constraints. Only invokes a solver when needed to explore alternate branches.

This strikes a balance:
- Speed of concrete execution (actual running)
- Path coverage of symbolic methods
- Without paying the full cost of traditional symbolic engines


The tension between exhaustive search (symbolic) and efficient execution (concrete) mirrors challenges in multi-agent systems:
- How do agents explore action spaces efficiently?
- When is it worth paying the cost of explicit reasoning vs. pattern matching?
- The "solver as oracle" pattern — invoked selectively, not continuously


Hybrid approaches often beat pure ones. EXE doesn't choose between concrete and symbolic — it uses concrete by default, symbolic when valuable.

---

*Read: March 1, 2026 — Papers We Love NYC talk by Michael Vaughn*
