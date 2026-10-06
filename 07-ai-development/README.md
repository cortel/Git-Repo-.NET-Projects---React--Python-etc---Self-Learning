# AI development in .NET

This track covers application features: model calls, structured results, retrieval and restricted tool use. [AI infrastructure](../15-agentic-ai-infrastructure/) covers running those features reliably over time. Follow [Start here](../00-roadmap/start-here.md) for the overall order.

## Core sequence

1. [Model API integration](./model-api-integration/): LLM basics, a .NET client, structured output, streaming and cancellation.
2. [Evaluation dataset](./evaluation-datasets/): define success for the first feature, then rerun cases on every meaningful change.
3. [RAG](./rag/): prepare documents, retrieve authorized evidence and answer with verifiable source references.
4. [Tool calling and agents](./tool-calling-and-agents/): typed functions, execution boundaries and a bounded loop.

Use [embeddings](./embeddings/) and [structured-output/prompt exercises](./prompts-and-structured-output/) when those stages expose a gap. Add [privacy](./privacy/), [prompt-injection defenses](./guardrails-and-prompt-injection/) and [latency/cost checks](./cost-latency-and-monitoring/) from the first applicable feature.

## Starting implementation choices

Use C# and ASP.NET Core with Microsoft.Extensions.AI, one provider and one retrieval store. Begin with deterministic fakes for contract tests. Reuse PostgreSQL; add pgvector for the retrieval exercise. Keep provider credentials on the backend.

Microsoft.Extensions.AI supplies chat/embedding abstractions and middleware, while Microsoft Agent Framework is a separate orchestration choice. Learning RAG does not require an agent framework. [Model client documentation](https://learn.microsoft.com/en-us/dotnet/ai/microsoft-extensions-ai), [Agent Framework](https://learn.microsoft.com/en-us/agent-framework/overview/).

## Optional depth

- [Local models](./local-models/): when deployment/privacy requirements justify them.
- [Python/data fundamentals](./python-and-data-fundamentals/) and [model training](./ml-and-training-fundamentals/): for a later ML specialization.
- [AI-assisted development](./ai-assisted-development/): practice review and verification of generated code.

These are available exercises, not prerequisites for building .NET AI features. Use the [curated references](../14-learning-material/curated-links.md) instead of collecting parallel courses.
