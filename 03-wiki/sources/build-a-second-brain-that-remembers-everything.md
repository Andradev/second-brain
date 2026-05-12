---
source_path: "01-raw/videos/processed/Build A Second Brain That Remembers Everything.md"
source_url: "https://www.youtube.com/watch?v=yke4fLQUsh4"
source_type: "youtube"
channel: "Matt Wolfe"
published: 2026-05-06
processed: 2026-05-11
---

# Build A Second Brain That Remembers Everything

Source path: `01-raw/videos/processed/Build A Second Brain That Remembers Everything.md`

Processed date: 2026-05-11

## Short Summary

Matt Wolfe demonstrates building an AI second brain around Obsidian, Codex, and Karpathy's LLM Wiki pattern. He expands the base wiki with a journal and CRM so that saved sources, personal reflections, and contact notes can ground future answers.

## Key Claims Or Observations

- A normal second brain can become a dumping ground unless it has a retrieval, synthesis, and review layer.
- The proposed system has three pillars: a wiki/knowledge base, a CRM, and a journal.
- The wiki ingests articles, YouTube transcripts, tweets, podcasts, and other saved materials; AI summarizes them, extracts entities/concepts, and cross-links them.
- Journal entries can be answered with grounding from wiki pages, prior journal entries, and CRM records.
- CRM entries store relationship context so future queries can recall how people are connected to events, ideas, and conversations.
- Automations can periodically process new raw files and optionally push the updated vault to GitHub.

## Relevant Entities

- [[03-wiki/entities/matt-wolfe|Matt Wolfe]]
- [[03-wiki/entities/andrej-karpathy|Andrej Karpathy]]
- [[03-wiki/entities/obsidian|Obsidian]]
- [[03-wiki/entities/codex|Codex]]
- OpenClaw
- Hostinger
- GitHub

## Relevant Concepts

- [[03-wiki/concepts/ai-second-brain|AI Second Brain]]
- [[03-wiki/concepts/llm-wiki-pattern|LLM Wiki Pattern]]
- [[03-wiki/concepts/obsidian-as-ai-frontend|Obsidian As AI Frontend]]
- [[03-wiki/concepts/ai-agent-crm|AI Agent CRM]]

## Contradictions, Tensions, Or Updates

- The source suggests moving processed raw files into a processed folder and adding YouTube channel names to original source frontmatter. The current vault schema now moves root-level ingested files to `01-raw/videos/processed/`, while preserving source contents and adding verified `channel` metadata to generated source summary pages instead.
- It broadens the wiki from source processing into a personal operating system with journal and CRM workflows; those folders are not yet part of this vault's schema.

## Open Questions

- Should this vault adopt `journal/` and `crm/` folders as durable conventions?
- Should a recurring automation process new root-level raw files on a schedule?
