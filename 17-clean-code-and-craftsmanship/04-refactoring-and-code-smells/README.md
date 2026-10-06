# refactoring and code smells

Status: planned.

## Goal

Remove duplication and coupling from a small legacy feature.

## Evidence of completion

- [ ] Protect existing behavior with characterization tests.
- [ ] Refactor in small verifiable steps and explain cohesion/coupling changes.
- [ ] Keep a change log showing why each abstraction exists.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.

## Focused mini-projects

- [long method](./long-method/)
- [feature envy](./feature-envy/)
- [shotgun surgery](./shotgun-surgery/)

## Combined project

Finish with the [topic integration project](./99-integration-project/) to practice the concepts together.
