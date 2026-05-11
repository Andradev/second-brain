# LLM Wiki Schema

This Obsidian vault follows Andrej Karpathy's LLM Wiki pattern: raw sources are preserved, the wiki is maintained by the LLM, and this file defines the operating conventions.

## Architecture

- `raw/` is the immutable source collection. Read from it, but do not modify, rename, or delete source files unless the user explicitly asks.
- `raw/assets/` is for locally downloaded images and attachments referenced by raw sources.
- `wiki/` is the LLM-maintained knowledge layer. Create, update, cross-link, and reconcile markdown pages here.
- `AGENTS.md` is the schema and workflow document. Update it only when the user asks to evolve the wiki conventions or when a durable convention has clearly emerged.

## Wiki Map

- `wiki/index.md` is the content-oriented catalog. Read it first when answering questions, then drill into relevant pages.
- `wiki/log.md` is the append-only chronological record of setup work, ingests, queries, and lint passes.
- `wiki/overview.md` is the high-level orientation page for the wiki.
- `wiki/synthesis.md` is the evolving cross-source synthesis.
- `wiki/sources/` contains one summary page per ingested source.
- `wiki/entities/` contains pages for people, organizations, projects, places, and other named entities.
- `wiki/concepts/` contains pages for concepts, themes, and recurring ideas.
- `wiki/comparisons/` contains comparison tables, contrastive analyses, and durable query outputs that compare multiple things.

## Naming And Links

- Use descriptive, lowercase, hyphenated filenames: `example-source-title.md`, `example-concept.md`.
- Use Obsidian links for wiki pages, including paths when helpful: `[[wiki/concepts/example-concept|Example Concept]]`.
- Prefer stable source references using vault-relative paths such as `raw/example-source.md`.
- Do not invent facts. Mark unknowns, open questions, and data gaps directly.

## Page Conventions

Source summary pages should generally include:

- Source path
- Processed date
- Short summary
- Key claims or observations
- Relevant entities
- Relevant concepts
- Contradictions, tensions, or updates to prior claims
- Open questions

For YouTube videos saved through the Obsidian Web Clipper, source summary pages should include YAML frontmatter with a `channel` field. Pull the channel name from the clipped source metadata or page content when available; if it is missing but the YouTube URL is present, look up the video page and use the channel name from YouTube. Do not invent the channel name; mark it as `unknown` and list it under open questions if it cannot be verified.

Entity and concept pages should generally include:

- One-line definition or description
- Current synthesis
- Supporting sources
- Related pages
- Open questions

## Index Maintenance

Keep `wiki/index.md` organized by category. Each listed page should have a link and a one-line description. Add metadata only when it helps navigation, such as processed date or source count.

## Log Format

Append entries to `wiki/log.md` with this prefix format:

```md
## [YYYY-MM-DD] type | Title
```

Use these log types:

- `setup`
- `ingest`
- `query`
- `lint`

Each entry should briefly state what changed, which pages were touched, and any follow-up questions.

## Workflows

### Ingest

When the user asks to ingest a source:

1. Read the new source from `raw/`.
2. Inspect local images from `raw/assets/` when they are relevant.
3. Create or update the matching page in `wiki/sources/`.
4. Update related entity, concept, comparison, overview, and synthesis pages as needed.
5. Cross-link any wiki pages generated or updated to the original source page
6. Update `wiki/index.md`.
7. Append an `ingest` entry to `wiki/log.md`.
8. Move the source file from the root raw/ directory to raw/processed

### Query

When answering a question:

1. Read `wiki/index.md` first.
2. Read relevant wiki pages.
3. Answer with citations to wiki pages and source paths when available.
4. If the answer has durable value, file it into the appropriate wiki page or create a new page, then update the index and log.

### Lint

When the user asks for a wiki health check:

1. Look for contradictions, stale claims, orphan pages, missing cross-references, important concepts without pages, and data gaps.
2. Suggest specific repairs or sources to seek.
3. Make straightforward maintenance updates when safe.
4. Append a `lint` entry to `wiki/log.md`.
