# 03 - RAG Systems

Document loading, text splitting, and full retrieval-augmented generation pipelines.

## Contents

| Resource | Original Path |
|----------|---------------|
| Document Loader | `GenAI_Project1_resources/1_document_loader/` |
| Text Splitter | `GenAI_Project1_resources/2_text_splitter/` |
| Real Estate Tool | See `07-projects/real-estate-rag` |
| Project resources | `GenAI_Project1_resources`, `GenAI_Project2_resources`, `GenAI_Project3_Resources` |

---

## Standard RAG Pipeline

```mermaid
flowchart TD
    A[Load Documents] --> B[Split into Chunks]
    B --> C[Embed Chunks]
    C --> D[(Vector Store)]
    E[User Query] --> F[Embed Query]
    F --> D
    D --> G[Retrieve Relevant Chunks]
    G --> H[Augment Prompt]
    H --> I[LLM Generate Answer]
```

---

## Learning Objectives

- Load PDFs, CSVs, URLs, etc.
- Choose appropriate text splitters
- Build and query a vector store
- Construct RAG chains with source attribution
- Add conversation memory to RAG
