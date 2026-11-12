# SHADDAI RAG Brain

Standalone RAG (Retrieval-Augmented Generation) knowledge base for the SHADDAI agent council.

## What's Inside

### Knowledge Bases (per agent)
- `data/rag/kb_shaddai/` — SHADDAI orchestrator knowledge
- `data/rag/kb_nexus/` — NEXUS technical knowledge
- `data/rag/kb_oracle/` — ORACLE research knowledge
- `data/rag/kb_zerox/` — ZEROX financial knowledge
- `data/rag/kb_turtle/` — TURTLE design knowledge
- `data/rag/kb_quill/` — QUILL writing knowledge
- `data/rag/kb_pikadon/` — PIKADON security knowledge

Each KB contains:
- `docs.json` — document chunks with embeddings
- `idf.json` — inverse document frequency scores

### RAG Engine
- `rag-index.js` — RAG indexing and search
- `rag-scrape.js` — web scraping for knowledge ingestion
- `concept-map.js` / `concept-map.json` — concept relationship mapping
- `lib/eco-brain.js` — brain/processing module

### Catalogs
- `data/skills-catalog.json` — full skills catalog
- `data/eco-workflows.json` — workflow definitions

## Usage

```bash
# Search the RAG brain
node rag-index.js --query "your question"

# Scrape new knowledge
node rag-scrape.js --url "https://example.com"
```

## Related
- Master MCP: https://github.com/IzzoSol/shaddai-mcp
- SHADDAI Signals: https://github.com/IzzoSol/shaddai-signals

*Built by Izzo (IzzoSol)*
'@