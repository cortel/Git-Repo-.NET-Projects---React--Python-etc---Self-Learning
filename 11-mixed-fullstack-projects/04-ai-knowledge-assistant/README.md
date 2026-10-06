# Document Q&A extension

Status: planned. Core stage 3 of [Start here](../../00-roadmap/start-here.md).

Extend the [inventory/order application](../02-inventory-and-orders/) with Q&A over synthetic support manuals. Store the brief, evaluation reports and retrieval experiments here; keep the integrated feature in the main codebase.

Use the [RAG lab](../../07-ai-development/rag/) as the single acceptance checklist. Required evidence: authorized retrieval, source support, abstention, document update/delete behavior and separate retrieval/answer measurements.

A separate chatbot application, additional vector stores and caching are optional. Avoid rebuilding the same pipeline under “PDF chatbot,” “RAG with .NET” and “enterprise Q&A” labels.
