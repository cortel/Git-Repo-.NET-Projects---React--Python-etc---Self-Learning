# Agentic operations extension

Status: planned. Stages 4-6 of [Start here](../../00-roadmap/start-here.md).

Extend the same [inventory/order application](../02-inventory-and-orders/) with an operations assistant over synthetic orders and incident/support records. This folder holds the capstone brief and evidence; it does not require a second application.

## Required evidence

- [ ] Compare a deterministic workflow with a bounded agent using restricted order/stock tools.
- [ ] Enforce schema validation, user/tenant permissions and step/time budgets server-side.
- [ ] Bind human approval to an exact simulated write and record the resulting effect.
- [ ] Persist accepted runs; demonstrate restart recovery and safe duplicate delivery.
- [ ] Handle cancellation and explain effects committed before cancellation.
- [ ] Show a React run/approval view, redacted trace and evaluation report.
- [ ] Demonstrate restore/rollback and defend design choices with an ADR and runbook.

MCP, multi-agent orchestration, generated-code execution, Redis and Kubernetes are optional follow-up experiments. Use existing [AI labs](../../07-ai-development/) and [infrastructure exercises](../../15-agentic-ai-infrastructure/) as needed; do not duplicate their checklists in separate mini-products.
