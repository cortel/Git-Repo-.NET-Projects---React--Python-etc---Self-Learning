# dependency scheduler

Status: planned combined project. No application code exists yet.

## Concepts combined

Graphs, priority queues, cancellation, profiling and SOLID

## Build in milestones

1. Schedule jobs with dependency validation and priority ordering.
2. Detect a cycle and cancel running work safely.
3. Measure throughput and explain the bottleneck.

## Required failure demonstration

A cyclic graph must be rejected without partially executing it.

## Completion evidence

- [ ] Explain requirements, invariants and component boundaries before implementation.
- [ ] Show a working end-to-end path and the required failure demonstration.
- [ ] Include appropriate automated checks or reproducible experiments and actual results.
- [ ] Document setup, run, verification and recovery commands where executable.
- [ ] Defend the chosen patterns against a simpler baseline and record limitations.
- [ ] Link commits, relevant topic exercises and an architecture diagram or decision record.

Use one source-code home. Prefer extending the inventory-and-orders application; this folder may contain only the integration brief and evidence linked to that implementation. Professional-practice projects produce reviewable artifacts as well as technical evidence. Use synthetic data and local infrastructure first; cloud deployment remains a separate authorized action.

Return to the [track exercises](../README.md).
