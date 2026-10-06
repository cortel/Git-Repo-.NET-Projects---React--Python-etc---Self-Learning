# legacy modernization delivery

Status: planned combined project. No application code exists yet.

## Concepts combined

Requirements, characterization, estimation, incremental migration, communication and postmortems

## Build in milestones

1. Write measurable acceptance criteria and capture legacy behavior.
2. Plan and deliver one reversible modernization slice.
3. Review a simulated incident and communicate changed scope.

## Required failure demonstration

A changed requirement must produce an explicit scope and risk decision supported by evidence.

## Completion evidence

- [ ] Explain requirements, invariants and component boundaries before implementation.
- [ ] Show a working end-to-end path and the required failure demonstration.
- [ ] Include appropriate automated checks or reproducible experiments and actual results.
- [ ] Document setup, run, verification and recovery commands where executable.
- [ ] Defend the chosen patterns against a simpler baseline and record limitations.
- [ ] Link commits, relevant topic exercises and an architecture diagram or decision record.

Use one source-code home. Prefer extending the inventory-and-orders application; this folder may contain only the integration brief and evidence linked to that implementation. Professional-practice projects produce reviewable artifacts as well as technical evidence. Use synthetic data and local infrastructure first; cloud deployment remains a separate authorized action.

Return to the [track exercises](../README.md).
