# order quality pipeline

Status: planned combined project. No application code exists yet.

## Concepts combined

TDD, unit tests, integration tests, contracts, properties and mutation testing

## Build in milestones

1. Develop stock invariants through red-green-refactor.
2. Verify persistence and an external provider contract.
3. Measure surviving mutations and close meaningful gaps.

## Required failure demonstration

A duplicate request and stock conflict must be caught at the appropriate test boundary.

## Completion evidence

- [ ] Explain requirements, invariants and component boundaries before implementation.
- [ ] Show a working end-to-end path and the required failure demonstration.
- [ ] Include appropriate automated checks or reproducible experiments and actual results.
- [ ] Document setup, run, verification and recovery commands where executable.
- [ ] Defend the chosen patterns against a simpler baseline and record limitations.
- [ ] Link commits, relevant topic exercises and an architecture diagram or decision record.

Use one source-code home. Prefer extending the inventory-and-orders application; this folder may contain only the integration brief and evidence linked to that implementation. Professional-practice projects produce reviewable artifacts as well as technical evidence. Use synthetic data and local infrastructure first; cloud deployment remains a separate authorized action.

Return to the [track exercises](../README.md).
