---
source_path: "raw/processed/llm-wiki.md"
source_url: "https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f"
source_type: "gist"
processed: 2026-05-11
---

# LLM Wiki

Source path: `raw/processed/llm-wiki.md`

Processed date: 2026-05-11

## Short Summary

Karpathy's LLM Wiki pattern proposes a personal knowledge base where raw sources are preserved and an LLM maintains a persistent, interlinked Markdown wiki on top of them. The wiki is not just retrieval: it accumulates summaries, entity pages, concept pages, contradictions, and cross-source synthesis over time.

## Key Claims Or Observations

- Standard RAG retrieves fragments at query time but does not accumulate durable synthesis.
- The LLM Wiki pattern compiles knowledge once into a maintained wiki, then keeps that wiki current as new sources arrive.
- The architecture has three layers: immutable raw sources, an LLM-maintained wiki, and a schema file that tells the agent how to operate.
- Core operations are ingest, query, and lint.
- The index is content-oriented and helps the LLM navigate; the log is chronological and records what happened.
- Obsidian can act as the human-facing IDE for the wiki while the LLM acts as the maintainer.

## Relevant Entities

- [[wiki/entities/andrej-karpathy|Andrej Karpathy]]
- [[wiki/entities/obsidian|Obsidian]]
- qmd
- Marp
- Dataview

## Relevant Concepts

- [[wiki/concepts/llm-wiki-pattern|LLM Wiki Pattern]]
- [[wiki/concepts/ai-second-brain|AI Second Brain]]
- [[wiki/concepts/obsidian-as-ai-frontend|Obsidian As AI Frontend]]
- [[wiki/concepts/company-brain|Company Brain]]

## Contradictions, Tensions, Or Updates

- The source positions the wiki as a compounding artifact rather than a transient chat or retrieval layer.
- It leaves implementation details intentionally open, so this vault's `AGENTS.md` is the local instantiation of the pattern.

## Open Questions

- Which optional tools, such as qmd, become worthwhile as this vault grows?
- How much should durable query answers be filed back into the wiki versus left only in chat?
