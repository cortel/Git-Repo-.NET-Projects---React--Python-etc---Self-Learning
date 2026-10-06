# recoverable approved operations agent

Status: planned combined project. No application code exists yet.

## Concepts combined

Bounded agent state, typed tools, tenancy, durable jobs, approval, audit, evaluation and quotas

## Build in milestones

1. Implement a deterministic baseline and stubbed bounded agent.
2. Persist checkpoints and bind write approval to exact arguments.
3. Crash and resume runs while enforcing permissions, cost and release gates.

## Required failure demonstration

Resume cannot repeat an approved external effect or broaden its approved scope.

## Completion evidence

- [ ] Explain requirements, invariants and component boundaries before implementation.
- [ ] Show a working end-to-end path and the required failure demonstration.
- [ ] Include appropriate automated checks or reproducible experiments and actual results.
- [ ] Document setup, run, verification and recovery commands where executable.
- [ ] Defend the chosen patterns against a simpler baseline and record limitations.
- [ ] Link commits, relevant topic exercises and an architecture diagram or decision record.

Use one source-code home. Prefer extending the inventory-and-orders application; this folder may contain only the integration brief and evidence linked to that implementation. Professional-practice projects produce reviewable artifacts as well as technical evidence. Use synthetic data and local infrastructure first; cloud deployment remains a separate authorized action.

Return to the [track exercises](../README.md).
