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

### **Research Direction**

My research builds edge-hosted cooperative intelligence for connected autonomous vehicles. Vehicles and roadside units share what they observe; an edge server fuses those observations into one shared world model per road locale, tracks the actors in it, predicts their trajectories, and returns the result to every vehicle planner. The systems question at the center of my work: shared state is only useful if it reaches the planner while it is still fresh, still correct, and still affordable on edge hardware. My research develops this stack along five directions.

**A platform to measure it.** [eCAV](https://arxiv.org/abs/2506.16535) is a distributed simulation platform that couples CARLA, containerized per-vehicle actors, a real edge inference service on real GPU hardware, and an ns-3 cellular radio plane under one deterministic clock, so wall-clock compute and network behavior are measured, not modeled.

**Correctness under latency.** When multiple sources report the same physical object at different delays, naive merging produces duplicates and identity swaps. I design freshness and provenance contracts for edge-merged state that separate failures caused by stale physics from failures caused by broken identity logic, and measure both in closed-loop driving.

**Scaling up under one GPU.** Fusing every available vehicle overruns the latency budget as participation grows. Conductor (ACM/IEEE SEC 2026) selects the vehicles that add evidence beyond the roadside unit's view and adapts prediction work each cycle, keeping the shared world model inside its freshness bound across traffic density.

**Scaling out across locales.** Vehicles cross locale boundaries, and the learned tracker state that describes them exists only at the source edge. I am building predictive migration of that state, using the stack's own trajectory predictions to move it ahead of the vehicle.

**Feeding the stack.** Contributor uplinks and direct vehicle-to-vehicle links differ in capacity and latency; planned work schedules which vehicle sends over which link to maximize prediction quality per transmitted byte.

## CV

### [CV](./cv.md)

## Accomplishments

### Papers and Talks

### [Papers and Talks](./papers_and_talks.md)
