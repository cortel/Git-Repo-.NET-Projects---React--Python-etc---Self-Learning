# reliable order api

Status: planned combined project. No application code exists yet.

## Concepts combined

ASP.NET Core, DI lifetimes, EF concurrency, cache-aside, Strategy and TDD

## Build in milestones

1. Implement order invariants test-first and persist orders.
2. Add interchangeable pricing policies and a cached catalog.
3. Exercise concurrent updates and dependency failures.

## Required failure demonstration

Two competing stock changes cannot silently overwrite one another.

## Completion evidence

- [ ] Explain requirements, invariants and component boundaries before implementation.
- [ ] Show a working end-to-end path and the required failure demonstration.
- [ ] Include appropriate automated checks or reproducible experiments and actual results.
- [ ] Document setup, run, verification and recovery commands where executable.
- [ ] Defend the chosen patterns against a simpler baseline and record limitations.
- [ ] Link commits, relevant topic exercises and an architecture diagram or decision record.

Use one source-code home. Prefer extending the inventory-and-orders application; this folder may contain only the integration brief and evidence linked to that implementation. Professional-practice projects produce reviewable artifacts as well as technical evidence. Use synthetic data and local infrastructure first; cloud deployment remains a separate authorized action.

Return to the [track exercises](../README.md).
