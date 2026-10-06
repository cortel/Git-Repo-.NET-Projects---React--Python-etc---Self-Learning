# characterization tests and test doubles

Status: planned.

## Goal

Safely change a legacy module with poorly understood behavior.

## Evidence of completion

- [ ] Capture existing behavior before refactoring.
- [ ] Choose fakes, stubs or mocks based on the boundary being tested.
- [ ] Explain intentional behavior changes and avoid mocking internal implementation steps.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.

## Focused mini-projects

- [legacy characterization](./legacy-characterization/)
- [fake versus mock](./fake-versus-mock/)
