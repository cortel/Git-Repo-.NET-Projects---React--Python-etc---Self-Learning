# extensible checkout

Status: planned combined project. No application code exists yet.

## Concepts combined

Strategy, Adapter, Decorator, Factory Method, State and anti-pattern refactoring

## Build in milestones

1. Start with a simple checkout and characterize its behavior.
2. Introduce patterns only for a real provider or policy variation.
3. Compare the final design against the simple baseline.

## Required failure demonstration

A failed payment cannot advance the order to paid or trigger duplicate notifications.

## Completion evidence

- [ ] Explain requirements, invariants and component boundaries before implementation.
- [ ] Show a working end-to-end path and the required failure demonstration.
- [ ] Include appropriate automated checks or reproducible experiments and actual results.
- [ ] Document setup, run, verification and recovery commands where executable.
- [ ] Defend the chosen patterns against a simpler baseline and record limitations.
- [ ] Link commits, relevant topic exercises and an architecture diagram or decision record.

Use one source-code home. Prefer extending the inventory-and-orders application; this folder may contain only the integration brief and evidence linked to that implementation. Professional-practice projects produce reviewable artifacts as well as technical evidence. Use synthetic data and local infrastructure first; cloud deployment remains a separate authorized action.

Return to the [track exercises](../README.md).
