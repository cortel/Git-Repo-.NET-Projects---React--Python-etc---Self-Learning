# identity permissions and tenancy

Status: planned.

## Goal

Give each run only the identity, tenant scope and capabilities it needs.

## Evidence of completion

- [ ] Test denied tool actions, expired credentials and cross-tenant reads.
- [ ] Do not trust tenant identifiers or permissions supplied by a model.
- [ ] Keep credentials outside model context and record auditable authorization decisions.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.

## Focused mini-projects

- [per tool authorization](./per-tool-authorization/)
