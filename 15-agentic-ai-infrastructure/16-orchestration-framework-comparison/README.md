# Optional orchestration framework comparison

Status: planned. Deferred until the [core path](../../00-roadmap/start-here.md) exposes an orchestration maintenance problem.

Compare the existing .NET worker/loop with one current .NET framework, starting from [Microsoft Agent Framework documentation](https://learn.microsoft.com/en-us/agent-framework/overview/). Check the package's support and release status first. Read [Semantic Kernel migration guidance](https://learn.microsoft.com/en-us/agent-framework/migration-guide/from-semantic-kernel) only when evaluating existing Semantic Kernel code.

- [ ] Use the same inputs, tools and evaluation cases in both implementations.
- [ ] Compare state management, approvals, telemetry, cancellation and crash behavior.
- [ ] Verify persistence/replay guarantees rather than inferring them from an “agent” API.
- [ ] Measure code complexity, operating cost and debugging effort.
- [ ] Keep or reject the framework with a concrete reason and an ADR.

Do not rebuild the project in Semantic Kernel, AutoGen, LangGraph and Temporal to complete this exercise. Python and other orchestrators remain separate optional depth.

## Focused mini-projects

- [single agent versus multi agent](./single-agent-versus-multi-agent/)

## Combined project

Finish with the [topic integration project](./99-integration-project/) to practice the concepts together.
