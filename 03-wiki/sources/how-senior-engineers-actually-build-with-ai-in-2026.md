---
source_path: "01-raw/videos/processed/How Senior Engineers Actually Build With AI in 2026  Build a Full Stack Systems Architecture App.md"
source_url: "https://www.youtube.com/watch?v=14RP8liACqo&t=2636s"
source_type: "youtube"
channel: "JavaScript Mastery"
published: 2026-05-01
processed: 2026-05-11
---

# How Senior Engineers Actually Build With AI in 2026

Source path: `01-raw/videos/processed/How Senior Engineers Actually Build With AI in 2026  Build a Full Stack Systems Architecture App.md`

Processed date: 2026-05-11

## Short Summary

JavaScript Mastery presents an architecture-first workflow for building a production-grade collaborative SaaS app with AI agents. The app, Ghost AI, lets users describe a system, map it onto a shared canvas, collaborate in real time, and generate technical specifications.

## Key Claims Or Observations

- The central thesis is that AI-assisted building fails when architecture, context, and project boundaries are weak.
- The workflow uses a `context/` folder with project overview, AI workflow rules, code standards, UI context, architecture context, progress tracker, and `AGENTS.md`.
- Feature work is driven by small feature specs, each telling the agent what to do, what not to touch, and how to verify completion.
- The stack includes Next.js, React, TypeScript, Tailwind, Clerk, Prisma/Postgres, Liveblocks, React Flow, Trigger.dev, Vercel Blob, and AI SDK/Gemini.
- Long-running AI generation is moved out of request handlers and into Trigger.dev background tasks with live status updates.
- The tutorial treats agent context, progress tracking, code review, and incremental verification as essential controls for serious AI builds.

## Relevant Entities

- [[03-wiki/entities/javascript-mastery|JavaScript Mastery]]
- [[03-wiki/entities/codex|Codex]]
- Clerk
- Liveblocks
- Trigger.dev
- Prisma
- React Flow
- Vercel
- CodeRabbit

## Relevant Concepts

- [[03-wiki/concepts/spec-driven-agentic-development|Spec-Driven Agentic Development]]
- [[03-wiki/concepts/agentic-coding-workflow|Agentic Coding Workflow]]
- [[03-wiki/concepts/design-systems-for-ai-codegen|Design Systems For AI Codegen]]
- [[03-wiki/concepts/agent-friendly-software|Agent-Friendly Software]]

## Contradictions, Tensions, Or Updates

- The source is less "vibe coding" and more "controlled delegation": it argues the speed of AI only pays off when project context and specs constrain the agent.
- It reinforces the vault's own `AGENTS.md` role as a durable behavior contract for future AI work.

## Open Questions

- Which parts of the six-file context system should be adapted for this vault's own maintenance workflow?
- The model and library versions mentioned in the video may become stale and should be checked before implementation.
