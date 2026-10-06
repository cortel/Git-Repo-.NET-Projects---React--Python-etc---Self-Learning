# operable order platform

Status: planned combined project. No application code exists yet.

## Concepts combined

Containers, CI artifacts, IaC, identity, deployment, telemetry and rollback

## Build in milestones

1. Run API, worker and database locally with health checks.
2. Build one immutable artifact and prepare environment configuration.
3. Inject a bad release, detect it and demonstrate local rollback.

## Required failure demonstration

Rollback must restore service without losing committed order data; cloud execution stays optional.

## Completion evidence

- [ ] Explain requirements, invariants and component boundaries before implementation.
- [ ] Show a working end-to-end path and the required failure demonstration.
- [ ] Include appropriate automated checks or reproducible experiments and actual results.
- [ ] Document setup, run, verification and recovery commands where executable.
- [ ] Defend the chosen patterns against a simpler baseline and record limitations.
- [ ] Link commits, relevant topic exercises and an architecture diagram or decision record.

Use one source-code home. Prefer extending the inventory-and-orders application; this folder may contain only the integration brief and evidence linked to that implementation. Professional-practice projects produce reviewable artifacts as well as technical evidence. Use synthetic data and local infrastructure first; cloud deployment remains a separate authorized action.

Return to the [track exercises](../README.md).
