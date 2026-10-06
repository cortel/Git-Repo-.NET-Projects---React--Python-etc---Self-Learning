# deployment and platform operations

Status: planned.

## Goal

Deploy API, workers, queue and checkpoint storage with reproducible configuration.

## Evidence of completion

- [ ] Start locally with Compose; add IaC and CI/CD when useful.
- [ ] Demonstrate graceful shutdown, schema migration, backup/restore and rollback.
- [ ] Explain autoscaling limits and worker-version compatibility for in-flight runs.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.

## Focused mini-projects

- [graceful worker drain](./graceful-worker-drain/)

## Combined project

Finish with the [topic integration project](./99-integration-project/) to practice the concepts together.
