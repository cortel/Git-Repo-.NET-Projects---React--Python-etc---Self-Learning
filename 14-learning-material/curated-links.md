# Curated resources and post review

Reviewed 6 October 2026. The repeated .NET Full-Stack Knowledge Hub post is one resource. The marketing copy is omitted; the useful concepts are mapped to the [single learning path](../00-roadmap/start-here.md).

## Placement and decisions

| Input | Placement | Decision |
| --- | --- | --- |
| .NET interview hubs | [Portfolio/interview practice](../12-professional-practice/portfolio-and-interviews/) | Use for recall and explanation after building; no second curriculum |
| GenAI fundamentals, .NET integration and RAG | [AI development](../07-ai-development/) | One measured feature, then one retrieval pipeline |
| Agent execution and operations | [AI infrastructure](../15-agentic-ai-infrastructure/) | Permissions, approvals, persistence, backpressure, evaluation and diagnostics |
| DDIA/distributed systems and concurrency | [Architecture](../10-architecture-and-system-design/) and [async lab](../02-dotnet-backend/async-concurrency-and-cancellation/) | Supporting depth when the application needs it |
| CV creator | Career utility | Excluded from the technical learning path |
| Angular | Separate frontend specialization | Deferred because this path prioritizes React |
| Redis, pgvector and Azure AI Search listed in sequence | Storage/operations choices | Select one retrieval store first; add caching or managed search only for a demonstrated need |
| Multi-agent systems and agentic RAG | Optional experiments | Compare against a simpler baseline; do not make them prerequisites |
| Evaluation/observability near the end | Cross-cutting requirements | Move to the first AI feature |

## Official references to use first

These are direct replacements for the four unusable source placeholders in the pasted post, not verified destinations of those placeholders.

| Need | Primary reference | Use |
| --- | --- | --- |
| LLM basics in C# | [Microsoft's Generative AI for Beginners .NET course](https://github.com/microsoft/Generative-AI-for-beginners-dotnet) | Read the relevant lesson, then implement a small feature |
| .NET model abstraction | [Microsoft.Extensions.AI](https://learn.microsoft.com/en-us/dotnet/ai/microsoft-extensions-ai) | Chat/embedding interfaces, DI and middleware |
| Retrieval concepts | [.NET RAG overview](https://learn.microsoft.com/en-us/dotnet/ai/conceptual/rag) | Understand ingestion, retrieval and source metadata |
| Retrieval exercise | [.NET vector-search walkthrough](https://learn.microsoft.com/en-us/dotnet/ai/quickstarts/build-vector-search-app) | Learn retrieval first; add answer generation and evaluation separately |
| Evaluation | [.NET evaluation libraries](https://learn.microsoft.com/en-us/dotnet/ai/evaluation/libraries) | Optional tooling for the required evaluation dataset |
| Agent orchestration | [Microsoft Agent Framework](https://learn.microsoft.com/en-us/agent-framework/overview/) | Consider when multi-step execution needs orchestration |
| C# async and bounded queues | [Async programming](https://learn.microsoft.com/en-us/dotnet/csharp/asynchronous-programming/), [Channels](https://learn.microsoft.com/en-us/dotnet/core/extensions/channels) | Practice cancellation, failures and admission limits |
| Tool interoperability | [MCP introduction](https://modelcontextprotocol.io/docs/getting-started/intro) | Use for tools shared across client/process boundaries |

Microsoft documents Agent Framework as the successor to its Semantic Kernel/AutoGen agent work. New exercises use current Agent Framework documentation when a framework is justified; Semantic Kernel remains useful to understand existing code. Do not study several orchestrators at once. Check package support and release status before adopting an example. [Microsoft overview](https://learn.microsoft.com/en-us/agent-framework/overview/), [migration guidance](https://learn.microsoft.com/en-us/agent-framework/migration-guide/from-semantic-kernel).

## Secondary resources from the posts

The shortened URLs were resolved through LinkedIn's public redirect page. Resource availability and content can change.

| Resource | Direct destination | Review status and role |
| --- | --- | --- |
| .NET Full-Stack Knowledge Hub | [dotnetfullstack.vercel.app](https://dotnetfullstack.vercel.app/) | Home and AI topic index inspected; use selected .NET/SQL/design questions. Angular is optional. Individual answers were not comprehensively audited |
| Senior .NET Interview Prep | [interview.liorsherbaty.com](https://interview.liorsherbaty.com/) | Home/course navigation inspected; use an explanation or coding drill after implementation. Full question bank not audited |
| Distributed Systems and DDIA | [ddia.liorsherbaty.com](https://ddia.liorsherbaty.com/) | Destination resolved; content could not be retrieved by the web reader. Retained as an unreviewed optional reference |
| .NET Concurrency | [concurrency.liorsherbaty.com](https://concurrency.liorsherbaty.com/) | Overview and selected Tasks/Channels sections inspected; reproduce examples and verify against official .NET documentation |
| CV Creator | [cv.liorsherbaty.com](https://cv.liorsherbaty.com/) | Destination resolved; no content review because it is outside this technical path |

No claim of complete correctness, currentness, free access or account requirements is made for the secondary sites. They supply practice prompts; official documentation and reproducible code settle technical questions.

## Useful additions retained from the hub

The AI topic index highlights streaming UI behavior, source citations, retrieval access control and index freshness. Those are now explicit acceptance checks in the existing labs. They are extensions of existing work, not more parallel projects.
