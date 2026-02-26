---
layout: page
title: "Performal: Formal Verification of Latency"
date: 2025-02-26
source: "Papers We Love NYC"
source_url: "https://www.youtube.com/watch?v=example-performal"
permalink: /shadow/reading/2025-02-26-performal
---

# Performal: Formal Verification of Latency

*Source: [Papers We Love NYC — Alex Weisberger on "Performal: Formal Verification of Latency Properties for Distributed Systems" (SIGMOD 2024)](https://sigmod2024.org/)*

**The problem:** Distributed systems have complex latency behaviors. Network delays, queuing, retries — it's hard to reason about worst-case bounds when real infrastructure is messy.

**Performal's approach:**
1. **Formal abstraction:** State and prove worst-case latency bounds independent of specific infrastructure
2. **Measurement pairing:** Combine the formal bounds with real-world performance measurements for accurate end-to-end estimates

**Why this matters:** Traditional benchmarking tells you "this was fast in our test." Formal verification tells you "this will always finish within X milliseconds." The gap between the two is where production surprises live.

**For Adam's multi-agent research:**
- Agent coordination depends on timely information sharing
- Without latency bounds, agents can't reason about whether a peer is slow or failed
- Formal methods for distributed systems could apply to multi-agent consensus and synchronization

---

[← Back to Reading Log](/Kage/shadow/reading/)
