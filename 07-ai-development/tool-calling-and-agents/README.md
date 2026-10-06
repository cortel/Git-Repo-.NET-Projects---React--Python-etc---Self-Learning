# Restricted tool calling and bounded agents

Status: planned. Core stage 4 of [Start here](../../00-roadmap/start-here.md).

Give the existing assistant typed tools for order status and stock lookup. The model proposes a tool call; application code validates and authorizes execution. Compare an explicit workflow with a bounded goal-directed loop.

## Acceptance checks

- [ ] Define precise tool names, schemas, descriptions and predictable error results.
- [ ] Scope queries to the authenticated user/tenant, parameterize inputs and cap returned rows.
- [ ] Use allowlisted read operations, not unrestricted model-generated SQL or arbitrary HTTP requests.
- [ ] Reject malformed arguments, unauthorized resources and unknown tools server-side.
- [ ] Test timeout, tool failure, inconsistent output, cancellation and exhausted step budgets.
- [ ] Add one simulated write with approval tied to the exact validated action.
- [ ] Record tool calls and effects in an audit trace, with sensitive data redacted.
- [ ] Run [evaluations](../evaluation-datasets/) against the workflow and agent and justify whether the agent adds value.

Function calling and tool calling describe the same basic integration concept here; they are not two separate courses. Long-term memory, autonomous plans, agentic RAG and multi-agent systems are deferred.

Use Microsoft.Extensions.AI for the first typed-function exercise. Consider [Microsoft Agent Framework](https://learn.microsoft.com/en-us/agent-framework/overview/) when orchestration warrants it. MCP is an optional second-client integration in [infrastructure](../../15-agentic-ai-infrastructure/05-tool-gateway-and-mcp/), not a prerequisite for tools.

## Focused mini-projects

- [typed tool calling](./typed-tool-calling/)
