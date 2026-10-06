# durable workflows and checkpoints

Status: planned.

## Goal

Persist workflow state so a process restart does not lose a long-running task.

## Evidence of completion

- [ ] Crash between steps and resume from persisted state.
- [ ] Record inputs and results of nondeterministic calls; do not assume re-running a model reproduces its output.
- [ ] Handle versioned workflow state and safe replay boundaries.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.

## Focused mini-projects

- [checkpoint and resume](./checkpoint-and-resume/)
