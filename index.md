---
layout: home
title: About Me
---

<img src="./1.png" width="200" />

**Senior Staff Software Engineer** | [Intel Corporation](https://www.intc.com/segments)

**PhD Student**\
[School of Computer Science](https://scs.gatech.edu/)\
[Embedded Pervasive Lab](https://epl.gatech.edu/)\
Advised by [Professor Umakishore Ramachandran](https://www.cc.gatech.edu/~rama/)\
[Georgia Institute of Technology](https://www.cc.gatech.edu/)

### Research

My research builds edge-hosted cooperative intelligence for connected autonomous vehicles: vehicles and roadside units share what they observe, and an edge server fuses those observations into one shared world model per road locale, tracks the actors in it, predicts their trajectories, and returns the result to every vehicle planner. Shared state is useful only if it reaches the planner while it is still fresh, still correct, and still affordable on edge hardware. My work treats those three constraints as the core systems problems.

* **[eCAV](https://arxiv.org/abs/2506.16535)** — a distributed simulation platform that measures real edge compute and simulated radio behavior inside one deterministic closed driving loop.
* **[Conductor](https://tlandle.github.io/conductor/)** *(ACM/IEEE SEC 2026)* — a deadline-aware edge service that keeps the shared world model fresh as vehicle participation grows, by selecting which vehicles contribute and how much prediction runs each cycle.
* **Correctness under latency** — freshness and provenance contracts that keep edge-merged state consistent when many sources report the same objects at different delays.
* **Service continuity across locales** — predictive migration of learned tracker state as vehicles move between edge servers.
* **Communication scheduling** — choosing which vehicle sends over which link to maximize prediction quality per transmitted byte.

### News

* **2026** — Conductor accepted at the ACM/IEEE Symposium on Edge Computing (SEC). [Project page](https://tlandle.github.io/conductor/).
* **2025** — eCAV, our edge-assisted evaluation platform for connected autonomous vehicles, is on [arXiv](https://arxiv.org/abs/2506.16535).

### More

[Curriculum Vitae](./cv.md) · [Publications & Talks](./papers_and_talks.md)
