# clean tests and concurrency

Status: planned.

## Goal

Write understandable tests for a bounded producer/consumer feature.

## Evidence of completion

- [ ] Separate deterministic unit behavior from concurrency integration tests.
- [ ] Test cancellation, completion, errors and a relevant shared-state race.
- [ ] Prefer controllable time and synchronization to arbitrary sleeps.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.
