---
title: "Sensitive Information Leakage from Tool-Call Traces"
collection: "publications"
category: "workshops"
permalink: "/publication/sensitive-information-leakage-tool-call-traces"
excerpt: "Inferring sensitive patient attributes from tool names alone in simulated healthcare-agent traces, without access to prompts, tool arguments, or outputs."
date: 2026-12-01
venue: "AIWild and InfPriv Workshops at NeurIPS"
publication_status: "Poster accepted at"
citation: "<b>Kook, J.</b>, Kim, S., and Vakudavathu, P. C. S. (2026). &quot;Sensitive Information Leakage from Tool-Call Traces.&quot; Poster accepted at the AIWild and InfPriv Workshops at NeurIPS, December 2026."
---

**Status:** Poster accepted at the AIWild and InfPriv Workshops at NeurIPS, December 2026.

**Authors:** Jihyung Kook, S. Kim, and P. C. S. Vakudavathu.

[Conference listing](https://neurips.cc/virtual/2026/loc/sydney/168249)

### Research focus
Can observable tool-call traces reveal sensitive information even when prompts, tool arguments, and outputs are hidden? This work studies that question using simulated healthcare-agent traces.

### My contribution
- Developed and evaluated three- and four-layer MLP classifiers on 3,190 simulated traces to infer sensitive patient attributes from tool names alone.
- Compared order-agnostic bag-of-tools frequency features with chronological n-gram features across three prediction tasks.
- Achieved a macro-F1 of 0.689 for treatment complexity, demonstrating leakage even without invocation-order information in this experimental setting.
