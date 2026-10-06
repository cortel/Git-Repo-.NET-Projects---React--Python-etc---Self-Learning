# Evaluated retrieval-augmented generation

Status: planned. Core stage 3 of [Start here](../../00-roadmap/start-here.md).

Extend the same application with Q&A over a few synthetic support manuals. First verify retrieval without a model-generated answer. Then add generation constrained by the returned evidence.

## Pipeline

Source documents → parsed text → chunks with source/version/access metadata → indexed retrieval → authorized evidence → generated answer with verifiable references.

## Acceptance checks

- [ ] Inspect extracted text, including tables and poor/missing text. Defer OCR until an actual source requires it.
- [ ] Make ingestion repeatable with document IDs, content hashes and explicit retry/error handling.
- [ ] Compare a keyword baseline with vector retrieval. Change chunking, overlap or top-K one at a time and measure the result.
- [ ] Use one embedding model and compatible index configuration; record dimensions and versions.
- [ ] Enforce document access at retrieval and before building model context; test a forbidden document.
- [ ] Trace references to actual source passages and expose them in React. A printed citation is not proof of support.
- [ ] Handle unsupported questions by abstaining rather than inventing an answer.
- [ ] Update and delete a document; verify old chunks stop being retrieved.
- [ ] Treat retrieved text as untrusted data and test an injected instruction.
- [ ] Report retrieval quality separately from answer correctness, latency and usage.

Use PostgreSQL plus pgvector as the first persistent vector option. Hybrid search and reranking are later experiments if measured retrieval quality needs improvement. Azure AI Search is an alternative storage/search exercise, not an additional mandatory layer; Redis is not required.

References: [.NET RAG concepts](https://learn.microsoft.com/en-us/dotnet/ai/conceptual/rag), [.NET vector-search walkthrough](https://learn.microsoft.com/en-us/dotnet/ai/quickstarts/build-vector-search-app). Keep application code in the existing project; this folder can hold focused experiments and evaluation evidence.
