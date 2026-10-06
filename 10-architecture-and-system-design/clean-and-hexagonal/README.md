# clean and hexagonal

Status: planned.

## Exercise

Build a focused, runnable example of clean and hexagonal using a concrete scenario. Demonstrate normal behavior and a relevant failure or edge case.

## Completion checklist

- [ ] Define the problem and acceptance criteria.
- [ ] Implement a small useful example.
- [ ] Document prerequisites and exact run commands.
- [ ] Verify behavior with appropriate tests or reproducible checks.
- [ ] Explain tradeoffs, alternatives, and when to use this approach.
- [ ] Record lessons and one follow-up improvement.

Keep code, tests, and notes in this folder. Start with the [project brief](../../13-project-templates/project-brief.md).

## Architecture depth

- [ ] Implement the same use case through HTTP and a console adapter without changing domain rules.
- [ ] Keep compile-time dependencies pointing toward application/domain policy.
- [ ] Place wiring in a composition root; distinguish runtime call direction from source dependencies.
- [ ] Demonstrate a presenter/humble-object boundary where useful and test business behavior independently.
- [ ] Compare with a simpler vertical slice and justify additional layers by concrete requirements.

Continue with [component cohesion/coupling](../component-cohesion-and-coupling/) and [architecture checks](../architecture-fitness-functions/).

## Focused mini-projects

- [clean architecture](./clean-architecture/)
- [ports and adapters](./ports-and-adapters/)

## Combined project

Finish with the [topic integration project](./99-integration-project/) to practice the concepts together.
