# Log

Append-only chronological record of wiki activity. Entries use the prefix format `## [YYYY-MM-DD] type | Title`.

## [2026-05-10] setup | Initial LLM Wiki architecture

- Created the raw source layer, wiki layer, and schema file.
- Created starter core pages: [[wiki/index|Index]], [[wiki/overview|Overview]], and [[wiki/synthesis|Synthesis]].
- Created wiki category folders for sources, entities, concepts, and comparisons.

## [2026-05-10] setup | YouTube channel metadata convention

- Updated `AGENTS.md` so ingested YouTube video source summaries include a verified `channel` frontmatter field.
- Follow-up: apply this convention when processing YouTube clips from `raw/`.

## [2026-05-10] ingest | Initial raw source batch

- Processed all 10 raw Markdown files into source summary pages under `wiki/sources/`.
- Added YouTube `channel` frontmatter to all generated YouTube source summaries using the clipped source metadata.
- Created related concept pages for second brains, LLM Wiki, Obsidian as AI frontend, agentic coding, spec-driven development, AI CRM, AI-native business models, company brains, agent-friendly software, design-system-guided codegen, and model aggregator platforms.
- Created entity pages for recurring creators, tools, and organizations, plus comparison pages for model aggregator alternatives and Antigravity/Claude Code role division.
- Updated [[wiki/index|Index]], [[wiki/overview|Overview]], and [[wiki/synthesis|Synthesis]].
- Follow-up: decide whether to add journal/CRM folders, a `raw/processed/` convention, or recurring ingestion automation.

## [2026-05-11] ingest | Reprocessed raw source batch

- Reprocessed the 10 root-level raw Markdown sources using the updated ingest workflow.
- Verified that all YouTube source summary pages in `wiki/sources/` include `channel` frontmatter.
- Updated source summary paths and processed dates to point at `raw/processed/`.
- Refreshed [[wiki/index|Index]], [[wiki/synthesis|Synthesis]], [[wiki/concepts/llm-wiki-pattern|LLM Wiki Pattern]], [[wiki/sources/build-a-second-brain-that-remembers-everything|Build A Second Brain That Remembers Everything]], and [[wiki/sources/ninguem-usa-obsidian-ia-do-jeito-certo-metodo-karpathy|Ninguem Usa Obsidian + IA do Jeito Certo]].
- Moved all processed root-level source files into `raw/processed/`.
- Follow-up: decide whether to create a recurring automation for new root-level raw files and whether journal/CRM folders should become first-class vault conventions.
