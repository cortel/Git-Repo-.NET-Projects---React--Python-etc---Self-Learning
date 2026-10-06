# security and adversarial testing

Status: planned.

## Goal

Threat-model malicious user input, retrieved documents and compromised tool results.

## Evidence of completion

- [ ] Test injected instructions, data exfiltration attempts and excessive tool privileges.
- [ ] Enforce policies at the execution boundary, independently of the prompt.
- [ ] Record failed attacks, residual risks and incident handling.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.

## Focused mini-projects

- [prompt injection boundary](./prompt-injection-boundary/)
