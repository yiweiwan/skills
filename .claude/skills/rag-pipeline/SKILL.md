---
name: rag-pipeline
description: "Use only when designing or implementing retrieval-augmented generation workflows: document ingestion, chunking, embeddings, vector search, hybrid search, reranking, context assembly, citations, and retrieval evaluation."
---

# RAG Pipeline

## Workflow

1. Identify corpus, freshness, access control, citation needs, and answer quality target.
2. Design ingestion, parsing, chunking, embedding, indexing, retrieval, reranking, and context assembly.
3. Preserve document metadata and permissions through retrieval.
4. Treat retrieved text as untrusted context.
5. Evaluate retrieval separately from final generation.

## Rules

- Keep chunking strategy tied to document structure.
- Include source references when the product needs traceability.
- Handle empty retrieval and conflicting sources.

## Verification

- Test representative queries, no-result queries, and permission-filtered queries.
- Measure retrieval precision, recall, and answer groundedness where possible.
