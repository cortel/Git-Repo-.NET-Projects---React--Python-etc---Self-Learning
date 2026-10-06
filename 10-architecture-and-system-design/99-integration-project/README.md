# ddd event driven orders with tdd

Status: planned combined project. No application code exists yet.

## Concepts combined

DDD aggregates, bounded contexts, TDD, modular monolith, domain events, outbox, inbox and CQRS

## Build in milestones

1. Model order and inventory invariants test-first within a modular monolith.
2. Publish committed integration events via an outbox and build an idempotent projection.
3. Inject crashes, duplicate and out-of-order delivery and document consistency.

## Required failure demonstration

A crash after the database commit must not lose the event or duplicate the business effect.

## Completion evidence

- [ ] Explain requirements, invariants and component boundaries before implementation.
- [ ] Show a working end-to-end path and the required failure demonstration.
- [ ] Include appropriate automated checks or reproducible experiments and actual results.
- [ ] Document setup, run, verification and recovery commands where executable.
- [ ] Defend the chosen patterns against a simpler baseline and record limitations.
- [ ] Link commits, relevant topic exercises and an architecture diagram or decision record.

Use one source-code home. Prefer extending the inventory-and-orders application; this folder may contain only the integration brief and evidence linked to that implementation. Professional-practice projects produce reviewable artifacts as well as technical evidence. Use synthetic data and local infrastructure first; cloud deployment remains a separate authorized action.

Return to the [track exercises](../README.md).
