# budgets quotas and reliability

Status: planned.

## Goal

Bound agent resource use and define a service-level objective for completed jobs.

## Evidence of completion

- [ ] Apply per-run and per-tenant time, token, tool-call and concurrency limits.
- [ ] Prevent runaway loops and retry storms during provider failures.
- [ ] Test cancellation, partial success, budget exhaustion and a kill switch.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.

## Focused mini-projects

- [per tenant quotas](./per-tenant-quotas/)
