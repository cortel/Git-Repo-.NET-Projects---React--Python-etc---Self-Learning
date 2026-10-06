# queues workers and backpressure

Status: planned.

## Goal

Use a queue and isolated workers to handle agent jobs without blocking HTTP requests.

## Evidence of completion

- [ ] Demonstrate job claiming, leases, bounded concurrency and worker recovery.
- [ ] Handle duplicated delivery with idempotency keys and an effect ledger.
- [ ] Show retries, jitter, poison messages and a dead-letter recovery process.
- [ ] Document setup, exact run/check commands, and relevant failure cases.
- [ ] Explain an alternative and the cost of the chosen approach.


Keep implementation and evidence in this folder. Create src/, tests/, docs/, or infra/ when needed.

## Focused mini-projects

- [worker lease and recovery](./worker-lease-and-recovery/)

## Combined project

Finish with the [topic integration project](./99-integration-project/) to practice the concepts together.
