# Async, concurrency and cancellation

Status: planned. Supporting lab for stages 1, 2 and 5 of [Start here](../../00-roadmap/start-here.md).

Use a synthetic order lookup and document-ingestion worker to learn lifetime and failure behavior.

- [ ] Explain I/O concurrency versus CPU parallelism; use async I/O without blocking waits.
- [ ] Propagate cancellation and deadlines; distinguish ending a wait from stopping the underlying work.
- [ ] Observe all owned task failures, including grouped work; do not detach request-scoped work.
- [ ] Use a bounded Channel with explicit capacity, producer/consumer ownership and shutdown behavior.
- [ ] Demonstrate overload, worker failure and graceful drain with reproducible checks.
- [ ] Explain why an in-memory queue does not establish durability; add persisted admission only for the restart-recovery stage.
- [ ] Profile before trying ValueTask or extra parallelism. Observables are optional for a stream-composition requirement.

Use official [async guidance](https://learn.microsoft.com/en-us/dotnet/csharp/asynchronous-programming/) and [Channels documentation](https://learn.microsoft.com/en-us/dotnet/core/extensions/channels). The [curated concurrency resource](../../14-learning-material/curated-links.md) supplies supplementary examples to reproduce, not another mandatory course.
