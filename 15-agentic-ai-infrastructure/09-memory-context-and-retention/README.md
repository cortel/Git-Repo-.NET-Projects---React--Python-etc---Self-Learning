# memory context and retention

Status: planned.

## Goal

Separate conversation context, run checkpoints, retrieval data and longer-term memory.

## Evidence of completion

- [ ] Define ownership, access control, retention, deletion and provenance for each store.
- [ ] Demonstrate context limits, summarization and stale-memory handling.
- [ ] Keep memory scoped to the appropriate user/tenant; test unauthorized retrieval.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.

## Focused mini-projects

- [memory expiry and deletion](./memory-expiry-and-deletion/)
