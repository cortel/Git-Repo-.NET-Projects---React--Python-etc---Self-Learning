# tracing metrics and cost

Status: planned.

## Goal

Connect frontend requests, workflow steps, model calls and tool effects in one trace.

## Evidence of completion

- [ ] Propagate correlation IDs and record latency, errors, queue delay and tool outcomes.
- [ ] Measure per-run tokens/cost and redact secrets and sensitive content.
- [ ] Create a dashboard and diagnose a seeded failure from telemetry.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.

## Focused mini-projects

- [run trace and token accounting](./run-trace-and-token-accounting/)

## Combined project

Finish with the [topic integration project](./99-integration-project/) to practice the concepts together.
