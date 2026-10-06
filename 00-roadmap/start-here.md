# Start here

Build one application, improve it in six stages, and use the rest of this repository as a reference library. The target is strong .NET backend and fullstack judgment with practical AI engineering, then evidence of Senior/Lead responsibilities.

## One application and one stack

Use [inventory and orders](../11-mixed-fullstack-projects/02-inventory-and-orders/) as the code home: an ASP.NET Core API, React with TypeScript, EF Core and PostgreSQL. Extend it with order-support summaries, document Q&A and an operations assistant. Use synthetic orders and manuals.

Keep one modular application. Use Docker Compose locally and GitHub Actions for CI. Choose one model provider; start with a fake client so contract tests run without paid calls. Add pgvector to the same database when vector retrieval becomes useful. This is a curriculum choice to reduce setup, not a claim that this stack fits every company. Use a supported SDK and record dependency versions when implementation starts.

If a target job requires SQL Server, do a focused SQL Server query-plan/locking lab later. React remains the frontend priority; Angular is outside this path.

## Six stages and exit criteria

| Stage | Implement in the same app | Move on when you can demonstrate |
| --- | --- | --- |
| 1. Deliver a reliable feature | Order creation, stock rules, React form, SQL persistence, authorization, tests and CI | A real invalid request, denied action, concurrent stock conflict and failed database call are handled; you can explain a query plan and one design tradeoff |
| 2. Add a measured AI feature | Summarize synthetic order-support notes through a .NET model client; stream the result to React | Validate structured results; support timeout/cancellation; keep credentials server-side; run an evaluation dataset and report quality, latency and usage |
| 3. Ground answers with RAG | Ingest synthetic manuals, retrieve authorized chunks and answer with source references | Measure retrieval separately from answer quality; demonstrate missing evidence, an unauthorized document, an updated document and a deleted document |
| 4. Add restricted tools | Read order status and stock through typed functions; compare a workflow with a bounded agent loop | Reject bad arguments and unauthorized calls server-side; cap steps and time; approve a simulated write; show whether the agent improves on the deterministic baseline |
| 5. Make execution recoverable | Persistent jobs, one worker, bounded admission, checkpoints and audit history | Recover after a process crash, handle duplicate delivery without duplicate effects, cancel a run and explain what happens to already committed work |
| 6. Operate and defend the system | Deployment, tracing, evaluation release checks, restore/rollback and design review | Diagnose a seeded failure, measure cost/latency, restore data, justify boundaries and communicate a risk or changed requirement clearly |

TDD, clean code and appropriate DDD run through all six stages. Start with a stock/order invariant: do not introduce every pattern, repository or layer just to check a box. Security, evaluation and observability start with the first AI feature.

## Use only the supporting material you need

- Stage 1: [TDD](../08-testing-and-quality/tdd-red-green-refactor/), [clean code](../17-clean-code-and-craftsmanship/), [DDD](../10-architecture-and-system-design/domain-driven-design/), [async/cancellation](../02-dotnet-backend/async-concurrency-and-cancellation/).
- Stages 2-4: [AI development](../07-ai-development/). Use its focused labs for model contracts, evaluation, RAG and tools.
- Stage 5: [agent infrastructure](../15-agentic-ai-infrastructure/). Learn state, persistence, workers, approvals and limits as the feature needs them.
- Stage 6 and throughout: [Senior/Lead evidence rubric](./intermediate-to-senior-lead.md) and [technical leadership exercises](../16-senior-lead-engineering/).

The [knowledge assistant](../11-mixed-fullstack-projects/04-ai-knowledge-assistant/) and [agentic operations platform](../11-mixed-fullstack-projects/08-agentic-operations-platform/) folders can hold extension briefs and evidence that point to the same code home. They do not require two more applications.

## Defer unless a requirement justifies it

Redis, Azure AI Search, multiple vector databases/providers, Semantic Kernel plus other orchestrators, multi-agent systems, agentic RAG, generated-code execution, Kubernetes, Kafka, microservices, event sourcing, model training and Python are optional depth. Pick one when a measured problem calls for it.

MCP is a tool-interoperability exercise: add it when a second client/process needs the same tools. It is not a required stage between RAG and production. Multi-agent work is not a seniority milestone.

## Learning rhythm

For each feature: state the requirement, implement a small slice, break it deliberately, verify the fix, and explain the decision. Complete one stage before expanding the stack.

After a working change, record a two-minute explanation: problem, decision, alternative, failure behavior and evidence. Use one interview question to expose a gap, then reproduce the issue in code. Avoid reading several hubs in parallel.

Track stage evidence in [progress.md](./progress.md). Use [curated resources](../14-learning-material/curated-links.md) when needed; a bookmarked link does not count as progress.
