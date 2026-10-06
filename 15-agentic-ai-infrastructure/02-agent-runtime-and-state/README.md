# agent runtime and state

Status: planned.

## Goal

Design a .NET API and worker that execute a bounded agent loop with an explicit run lifecycle.

## Evidence of completion

- [ ] Model queued, running, awaiting approval, completed, failed, and cancelled states.
- [ ] Use typed tool inputs, structured outputs, step limits, deadlines and cancellation.
- [ ] Separate deterministic business rules from model decisions.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.
