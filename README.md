# GenAI Learning Lab

**Industry-style structured learning repository** for Generative AI, RAG, Agents, MCP, CrewAI, and practical projects.

This repo reorganizes materials from the raw course dump ([bode_casics_aigen](https://github.com/yash9614/bode_casics_aigen)) into a clean, professional format with:
- Clear learning objectives
- Architecture diagrams (Mermaid)
- Setup instructions
- Key concepts
- Project breakdowns
- Links back to original notebooks/code

> **How to use:** Work through the modules in order. Read each README before running code. Copy notebooks or code into your own working directory as needed. Original materials remain untouched in the source repo.

---

## Learning Path Overview

| Stage | Module | Focus | Level |
|-------|--------|-------|-------|
| 1 | [01-foundations](./01-foundations) | LLM calls, parameters, prompt engineering | Beginner |
| 2 | [02-vector-databases](./02-vector-databases) | ChromaDB, embeddings, metadata filtering | Beginner–Medium |
| 3 | [03-rag-systems](./03-rag-systems) | Document loaders, text splitters, full RAG pipelines | Medium |
| 4 | [04-agents-and-tools](./04-agents-and-tools) | Tool calling, semantic routers, SQL agents | Medium |
| 5 | [05-multi-agent](./05-multi-agent) | CrewAI crews, email agents, collaboration | Medium–Advanced |
| 6 | [06-mcp](./06-mcp) | Model Context Protocol servers & clients | Advanced |
| 7 | [07-projects](./07-projects) | End-to-end projects (Real Estate, E-commerce, Leave Management, Finance) | Medium–Advanced |
| 8 | [08-fine-tuning](./08-fine-tuning) | Fine-tuning exercises | Advanced |
| 9 | [course-agents](./course-agents) | Structured agent course (from course-gen-ai-main) | Advanced |

---

## Key Projects You Should Build

1. **Real Estate Research Tool** — URL → RAG with Streamlit (Exercise 5)
2. **E-commerce Chatbot** — Semantic router for FAQ + SQL product queries (Exercise 6 + Flipkart SOW)
3. **Leave Management MCP Server** — MCP tools for HR leave queries
4. **CrewAI Marketing / Email Agents** — Multi-agent collaboration
5. **Finance Data Extractor** — Simple GenAI data pipeline

See each project folder under `07-projects` for architecture and objectives.

---

## Tech Stack Across Materials

- **LLMs:** Llama via Groq, OpenAI-compatible
- **Frameworks:** LangChain, CrewAI, MCP
- **Vector DBs:** ChromaDB
- **Frontend:** Streamlit
- **Databases:** SQLite
- **Embeddings:** Hugging Face
- **Package management:** uv / pip

---

## Setup Recommendations

```bash
# Use uv for modern projects
uv init my-project
uv add langchain langchain-groq chromadb streamlit

# Or classic
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

Always use `.env` for API keys (GROQ_API_KEY, etc.). Never commit secrets.

---

## Original Source

Materials curated from [bode_casics_aigen](https://github.com/yash9614/bode_casics_aigen).  
Copyright notices on many solutions belong to Codebasics Inc. / LearnerX. Use for personal learning.

Happy building!
