# architecture fitness functions

Status: planned.

## Goal

Protect important architectural properties with executable checks.

## Evidence of completion

- [ ] Verify inward dependencies and prevent domain code from importing framework/persistence code.
- [ ] Add a useful contract compatibility or dependency-cycle check.
- [ ] Document which architectural requirements are enforced and which still need review.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.
