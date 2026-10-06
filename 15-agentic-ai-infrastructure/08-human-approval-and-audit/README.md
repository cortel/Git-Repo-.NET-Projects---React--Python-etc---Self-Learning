# human approval and audit

Status: planned.

## Goal

Require a human decision before a simulated external side effect.

## Evidence of completion

- [ ] Persist the exact proposed action and the approval decision.
- [ ] Prevent a changed action, expired approval or reused approval from executing.
- [ ] Resume after worker restart and show a traceable audit record.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.

## Focused mini-projects

- [approval state machine](./approval-state-machine/)

## Combined project

Finish with the [topic integration project](./99-integration-project/) to practice the concepts together.
