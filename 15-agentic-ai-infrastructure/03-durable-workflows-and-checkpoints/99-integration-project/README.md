# Combined project: 03 durable workflows and checkpoints

Status: planned integration exercise; no implementation yet.

## Scope

Combine the linked exercises below into one coherent scenario from the parent topic. Reuse the order application where it fits; otherwise use one small local harness or evidence package. Keep one implementation home and link to it rather than copying services into every exercise.

## Concepts and prerequisite exercises

- [checkpoint-and-resume](../checkpoint-and-resume/)

## Milestones

1. State a concrete scenario, the shared contracts and the observable outcomes. Demonstrate the simplest baseline first.
2. Integrate the relevant linked concepts incrementally. Explain why each selected concept is needed; an unused pattern is not a completion requirement.
3. Exercise their interaction: inject a failure at a boundary, observe its effect on the other components and demonstrate recovery or an explicit limitation.

## Completion evidence

- [ ] Record a normal end-to-end trace or walkthrough through the combined components.
- [ ] Demonstrate a boundary failure and verify the resulting state; avoid claiming delivery guarantees without evidence.
- [ ] Supply setup/run/check commands for executable work, or reviewable artifacts and acceptance criteria for configuration and leadership exercises.
- [ ] Explain one interaction tradeoff and compare a simpler design.
- [ ] Link source code, checks and measured evidence; mark the project planned until those exist.

Keep scope within this topic. Use the track-level integration project for the broader combination. Infrastructure work starts locally; cloud deployment and paid resources require separate authorization.
