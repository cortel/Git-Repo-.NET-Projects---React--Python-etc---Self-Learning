# model routing and gateways

Status: planned.

## Goal

Route model requests through a provider abstraction with explicit capability requirements.

## Evidence of completion

- [ ] Use a fake provider first; record model, prompt and configuration versions.
- [ ] Demonstrate timeouts, rate-limit handling and capability-compatible fallback.
- [ ] Evaluate fallback quality and reconcile token usage rather than assuming providers behave identically.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.
