# evaluations and release gates

Status: planned.

## Goal

Create regression evidence for an agent before releasing it.

## Evidence of completion

- [ ] Include successful tasks, denied actions, prompt injections and recovery cases.
- [ ] Compare with a deterministic baseline using task completion and side-effect correctness.
- [ ] Separate deterministic assertions, sampled model runs and optional model-based scoring.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.
