# evaluated document assistant

Status: planned combined project. No application code exists yet.

## Concepts combined

Structured output, embeddings, RAG, ACL filtering, citations and evaluations

## Build in milestones

1. Ingest synthetic manuals and version a question set.
2. Return authorized citations or abstain and measure results.
3. Handle index changes, model failures and bounded cost.

## Required failure demonstration

A deleted or unauthorized document must never support an answer.

## Completion evidence

- [ ] Explain requirements, invariants and component boundaries before implementation.
- [ ] Show a working end-to-end path and the required failure demonstration.
- [ ] Include appropriate automated checks or reproducible experiments and actual results.
- [ ] Document setup, run, verification and recovery commands where executable.
- [ ] Defend the chosen patterns against a simpler baseline and record limitations.
- [ ] Link commits, relevant topic exercises and an architecture diagram or decision record.

Use one source-code home. Prefer extending the inventory-and-orders application; this folder may contain only the integration brief and evidence linked to that implementation. Professional-practice projects produce reviewable artifacts as well as technical evidence. Use synthetic data and local infrastructure first; cloud deployment remains a separate authorized action.

Return to the [track exercises](../README.md).
