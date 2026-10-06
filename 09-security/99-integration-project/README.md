# tenant safe order service

Status: planned combined project. No application code exists yet.

## Concepts combined

Threat modeling, identity, object authorization, tenant isolation, input handling and audit

## Build in milestones

1. Model trust boundaries and implement scoped access.
2. Exercise local injection and cross-tenant abuse cases.
3. Verify audit redaction and credential rotation with synthetic secrets.

## Required failure demonstration

Changing a resource ID or tenant field must not bypass server-side authorization.

## Completion evidence

- [ ] Explain requirements, invariants and component boundaries before implementation.
- [ ] Show a working end-to-end path and the required failure demonstration.
- [ ] Include appropriate automated checks or reproducible experiments and actual results.
- [ ] Document setup, run, verification and recovery commands where executable.
- [ ] Defend the chosen patterns against a simpler baseline and record limitations.
- [ ] Link commits, relevant topic exercises and an architecture diagram or decision record.

Use one source-code home. Prefer extending the inventory-and-orders application; this folder may contain only the integration brief and evidence linked to that implementation. Professional-practice projects produce reviewable artifacts as well as technical evidence. Use synthetic data and local infrastructure first; cloud deployment remains a separate authorized action.

Return to the [track exercises](../README.md).
