# Agentic AI infrastructure

This track covers execution and operations: persisted state, workers, access boundaries, approvals and recovery. Model calls and RAG live in [AI development](../07-ai-development/). Follow [Start here](../00-roadmap/start-here.md); folder numbers are stable identifiers, not a mandatory learning sequence.

## Start early with every AI feature

- [Evaluation and release gates](./11-evaluations-and-release-gates/)
- [Tracing, metrics and cost](./12-tracing-metrics-and-cost/)
- [Security and adversarial tests](./13-security-and-adversarial-testing/)
- [Budgets and limits](./15-budgets-quotas-and-reliability/)

Begin with a small dataset, useful logs, authorization checks and bounded requests. Add operational sophistication as requirements grow.

## Core execution work

1. [Workflow versus agent](./01-workflows-versus-agents/): compare with a deterministic baseline.
2. [Identity and permissions](./06-identity-permissions-and-tenancy/): enforce authority outside the model.
3. [Approval and audit](./08-human-approval-and-audit/): bind approval to an exact proposed effect.
4. [Run state](./02-agent-runtime-and-state/): explicit lifecycle, deadlines and cancellation.
5. [Persistence and checkpoints](./03-durable-workflows-and-checkpoints/): demonstrate crash recovery.
6. [Queue workers and backpressure](./04-queues-workers-and-backpressure/): claims, retries and duplicate handling.
7. [Deployment and operations](./14-deployment-and-platform-operations/): rollbacks, shutdown and restore.

Use one worker and one persistence/queue approach initially. In-memory Channels teach flow control; work that must survive a process restart needs persisted admission/state. Do not treat the two as equivalent. [Official Channels documentation](https://learn.microsoft.com/en-us/dotnet/core/extensions/channels).

## Add only when needed

| Exercise | Trigger |
| --- | --- |
| [Tool gateway and MCP](./05-tool-gateway-and-mcp/) | A second client/process needs the same capability |
| [Sandboxing](./07-sandboxing-and-isolated-execution/) | You intentionally permit generated code or commands |
| [Memory and retention](./09-memory-context-and-retention/) | Information must outlive one conversation/run |
| [Routing and gateways](./10-model-routing-and-gateways/) | A measured availability/capability requirement needs multiple providers |
| [Framework comparison](./16-orchestration-framework-comparison/) | Maintaining custom orchestration has a concrete cost |

For a .NET framework exercise, use current [Microsoft Agent Framework documentation](https://learn.microsoft.com/en-us/agent-framework/overview/). It is not required for the first model call, retrieval feature or typed tool.

[LangGraph persistence](https://docs.langchain.com/oss/python/langgraph/persistence) and [Temporal execution](https://docs.temporal.io/workflow-execution) remain optional comparison references. Do not add Python or several orchestrators to the core .NET path. Protocol references: [MCP](https://modelcontextprotocol.io/docs/getting-started/intro); telemetry: [OpenTelemetry](https://opentelemetry.io/docs/).

Examples and release status change. Record tested dependency versions when implementing rather than copying old post snippets.

## Final combined project

- [recoverable-approved-operations-agent](./99-integration-project/) — Bounded agent state, typed tools, tenancy, durable jobs, approval, audit, evaluation and quotas
