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

I work in computer systems, with a focus on distributed systems and edge computing. The common thread in my work is systems that act on the physical world under a deadline: the useful lifetime of data is short, compute sits outside the data center, and correctness depends on when a result arrives, not only on what it says. Before autonomous vehicles, this led me to geo-distributed publish-subscribe systems (ePulsar, SEC 2021). My industry background is in operating systems, virtualization, and embedded platforms, which shapes how I build and evaluate research systems: real code, real hardware, measured behavior.

My current work applies this to connected autonomous vehicles. Vehicles and roadside units share observations. An edge server fuses them into one world model per road region, tracks the actors in it, predicts their trajectories, and returns the result to each vehicle planner. The shared state must reach the planner while it is still fresh, still correct, and within the compute budget of edge hardware. My research addresses these three constraints.

* [eCAV](https://arxiv.org/abs/2506.16535) is a distributed simulation platform. It measures real edge compute and simulated radio behavior in one deterministic closed driving loop.
* [Conductor](https://tlandle.github.io/conductor/) (ACM/IEEE SEC 2026) is a deadline-aware edge service. It selects which vehicles contribute to fusion and how much prediction runs on each cycle, keeping the world model fresh as participation grows.
* Correctness under latency. I design contracts that keep merged state consistent when several sources report the same objects at different delays.
* Service continuity. Learned tracker state migrates ahead of a vehicle as it moves between edge servers.
* Communication scheduling. Each vehicle sends over the link that adds the most prediction quality per transmitted byte.

### News

* 2026. Conductor was accepted at the ACM/IEEE Symposium on Edge Computing (SEC). [Project page](https://tlandle.github.io/conductor/).
* 2025. eCAV is on [arXiv](https://arxiv.org/abs/2506.16535).

### More

[Curriculum Vitae](./cv.md) · [Publications & Talks](./papers_and_talks.md)
