# LLM Wiki Pattern

The LLM Wiki pattern is a knowledge-base architecture where an LLM maintains a persistent, interlinked wiki on top of immutable raw sources.

## Current Synthesis

The pattern has three layers: `raw/` for preserved sources, `wiki/` for LLM-maintained synthesis, and `AGENTS.md` for operating rules. Its core advantage over one-off RAG is compounding: summaries, contradictions, entity pages, concept pages, and query outputs remain in the wiki instead of being rediscovered every chat.

The current vault implements the pattern with source pages, entity pages, concept pages, comparison pages, an index, a synthesis page, and an append-only log. Legacy raw files are preserved in `01-raw/imports/legacy/raw-originals/` and classified copies move to the appropriate category, such as `01-raw/videos/processed/` or `01-raw/articles/processed/`.

## Supporting Sources

- [[03-wiki/sources/llm-wiki|LLM Wiki]]
- [[03-wiki/sources/ninguem-usa-obsidian-ia-do-jeito-certo-metodo-karpathy|Ninguem Usa Obsidian + IA do Jeito Certo]]
- [[03-wiki/sources/build-a-second-brain-that-remembers-everything|Build A Second Brain That Remembers Everything]]

## Related Pages

- [[03-wiki/concepts/ai-second-brain|AI Second Brain]]
- [[03-wiki/concepts/obsidian-as-ai-frontend|Obsidian As AI Frontend]]
- [[03-wiki/entities/andrej-karpathy|Andrej Karpathy]]

## Open Questions

- When should query answers become durable pages?
- Should processed status also be exposed through source-page metadata, Dataview queries, or automation reports?
