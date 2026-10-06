# Model API integration in .NET

Status: planned. Core stage 2 of [Start here](../../00-roadmap/start-here.md).

Add a synthetic order-support summary to the existing inventory application. Learn tokens, context limits, message roles, sampling, hallucinations and structured output through this feature. Sampling controls are provider/model dependent; validate actual capabilities rather than assuming every setting is supported.

## Acceptance checks

- [ ] Use a fake .NET chat client first, then one real provider through Microsoft.Extensions.AI.
- [ ] Bound input/context and output; keep a useful failure contract for oversized requests.
- [ ] Validate a structured summary against the application's schema and business constraints. Valid JSON alone is not evidence that the result is correct.
- [ ] Stream responses through the backend to React, with explicit started/completed/failed states.
- [ ] Let the user stop a request; propagate cancellation and handle timeouts and partial output.
- [ ] Keep secrets server-side, redact logs and render model content without unsafe HTML.
- [ ] Record latency, token usage where available and prompt/model/configuration versions.
- [ ] Run the [evaluation cases](../evaluation-datasets/) before changing providers, prompts or models.

Use [Microsoft.Extensions.AI documentation](https://learn.microsoft.com/en-us/dotnet/ai/microsoft-extensions-ai) and the relevant lesson in [Microsoft's .NET course](https://github.com/microsoft/Generative-AI-for-beginners-dotnet). A second provider, fine-tuning and a standalone chat product are deferred.
