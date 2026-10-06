# concurrent order store

Status: planned combined project. No application code exists yet.

## Concepts combined

Schema design, transactions, indexes, migrations, backup and restore

## Build in milestones

1. Model stock and order consistency with concurrent clients.
2. Measure query plans and perform an expand-contract migration.
3. Restore a backup and verify data integrity.

## Required failure demonstration

Concurrent orders must preserve stock rules and a restored database must pass known integrity checks.

## Completion evidence

- [ ] Explain requirements, invariants and component boundaries before implementation.
- [ ] Show a working end-to-end path and the required failure demonstration.
- [ ] Include appropriate automated checks or reproducible experiments and actual results.
- [ ] Document setup, run, verification and recovery commands where executable.
- [ ] Defend the chosen patterns against a simpler baseline and record limitations.
- [ ] Link commits, relevant topic exercises and an architecture diagram or decision record.

Use one source-code home. Prefer extending the inventory-and-orders application; this folder may contain only the integration brief and evidence linked to that implementation. Professional-practice projects produce reviewable artifacts as well as technical evidence. Use synthetic data and local infrastructure first; cloud deployment remains a separate authorized action.

Return to the [track exercises](../README.md).
