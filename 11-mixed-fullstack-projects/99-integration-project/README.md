# fullstack order platform

Status: planned combined project. No application code exists yet.

## Concepts combined

.NET, React, DDD, TDD, PostgreSQL, event-driven integration, CI and telemetry

## Build in milestones

1. Deliver an authenticated order slice end to end.
2. Extend it with reliable events and observable background processing.
3. Add evaluated AI support only after the core is reliable.

## Required failure demonstration

Demonstrate concurrent users, denied access, duplicate delivery and a recoverable worker crash.

## Completion evidence

- [ ] Explain requirements, invariants and component boundaries before implementation.
- [ ] Show a working end-to-end path and the required failure demonstration.
- [ ] Include appropriate automated checks or reproducible experiments and actual results.
- [ ] Document setup, run, verification and recovery commands where executable.
- [ ] Defend the chosen patterns against a simpler baseline and record limitations.
- [ ] Link commits, relevant topic exercises and an architecture diagram or decision record.

Use one source-code home. Prefer extending the inventory-and-orders application; this folder may contain only the integration brief and evidence linked to that implementation. Professional-practice projects produce reviewable artifacts as well as technical evidence. Use synthetic data and local infrastructure first; cloud deployment remains a separate authorized action.

Return to the [track exercises](../README.md).
