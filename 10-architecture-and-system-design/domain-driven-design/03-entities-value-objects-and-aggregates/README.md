# entities value objects and aggregates

Status: planned.

## Goal

Implement an order aggregate with protected invariants.

## Evidence of completion

- [ ] Distinguish identity from value equality.
- [ ] Prevent invalid state and test aggregate boundaries under concurrent changes.
- [ ] Choose transactional consistency boundaries from domain rules.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.

## Focused mini-projects

- [entity](./entity/)
- [value object](./value-object/)
- [aggregate](./aggregate/)

## Combined project

Finish with the [topic integration project](./99-integration-project/) to practice the concepts together.
