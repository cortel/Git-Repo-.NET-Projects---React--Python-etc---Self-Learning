# Evaluation dataset and regression checks

Status: planned. Start with the first AI feature and extend through RAG and tools.

Create a small version-controlled synthetic dataset, initially around 20 cases. That is a manageable learning starting point, not a production sufficiency claim. Record input, expected behavior, relevant evidence and scoring criteria.

## Acceptance checks

- [ ] Separate ordinary cases, missing information, malformed output, forbidden requests and provider failures.
- [ ] Use deterministic fakes for application contracts; run separate sampled real-model evaluations for output quality.
- [ ] For retrieval, label relevant document/chunk IDs and measure retrieval quality independently of answer quality.
- [ ] For answers, inspect source support, factual errors and appropriate abstention.
- [ ] For tools, check chosen operation, validated arguments, authorization and actual effects.
- [ ] Define pass/fail criteria before tuning. Authorization bypass and duplicate effects are hard failures, not averaged quality scores.
- [ ] Compare the AI feature with a useful deterministic baseline.
- [ ] Record dataset, prompt, model, embedding and configuration versions, plus latency and usage.
- [ ] Keep a held-out set so tuning against the development cases does not become the only evidence.
- [ ] Explain the dataset's coverage limits; optional model judges need calibration against human review.

[Microsoft's evaluation libraries](https://learn.microsoft.com/en-us/dotnet/ai/evaluation/libraries) can support reporting and metrics. Learning success does not require installing every evaluator or using exact text matching for nondeterministic responses.
