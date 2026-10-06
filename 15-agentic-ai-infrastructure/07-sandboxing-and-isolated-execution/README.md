# sandboxing and isolated execution

Status: planned.

## Goal

Run potentially untrusted generated code or commands in a disposable environment.

## Evidence of completion

- [ ] Apply filesystem and network restrictions, resource limits and execution deadlines.
- [ ] Demonstrate blocked filesystem escape and outbound access.
- [ ] Explain why ordinary containers alone do not guarantee a sufficient hostile-code security boundary.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.

## Focused mini-projects

- [isolated execution](./isolated-execution/)
