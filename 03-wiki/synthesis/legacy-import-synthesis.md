# Synthesis

This page holds the evolving cross-source synthesis.

## Current Synthesis

The first source batch converges on one durable idea: AI work is mostly context work. Whether the task is maintaining a second brain, building software, running a WhatsApp agent, comparing AI platforms, or designing a business, the differentiator is not just model access. It is the quality of the source material, schemas, specs, workflows, memory, and review loops around the model.

[[03-wiki/concepts/llm-wiki-pattern|LLM Wiki Pattern]] is the organizing pattern for this vault. Raw sources stay preserved, while the wiki layer accumulates summaries, concepts, entities, comparisons, and synthesis. [[03-wiki/sources/llm-wiki|Karpathy's gist]] gives the architecture; [[03-wiki/sources/ninguem-usa-obsidian-ia-do-jeito-certo-metodo-karpathy|Hora de Codar]] and [[03-wiki/sources/build-a-second-brain-that-remembers-everything|Matt Wolfe]] show practical Obsidian/Codex/Claude Code versions.

The [[03-wiki/concepts/ai-second-brain|AI Second Brain]] sources split into manual and AI-maintained approaches. [[03-wiki/sources/o-minimo-para-nao-viver-perdido-na-vida-crie-um-segundo-cerebro|Node's tutorial]] emphasizes capture, linking, and review habits. The LLM Wiki sources add an agent that performs the tedious maintenance: summarizing, linking, extracting entities, and filing durable query answers.

The AI coding sources agree that agents need boundaries. [[03-wiki/sources/how-senior-engineers-actually-build-with-ai-in-2026|JavaScript Mastery]] makes the strongest case for [[03-wiki/concepts/spec-driven-agentic-development|Spec-Driven Agentic Development]]: context files, feature specs, progress tracking, and verification. [[03-wiki/sources/antigravity-com-claude-code-e-absurdo-crie-um-crm-completo|Felipe Borges]] emphasizes a practical split between [[03-wiki/entities/google-antigravity|Google Antigravity]] as visual workspace and [[03-wiki/entities/claude-code|Claude Code]] as implementation agent. [[03-wiki/sources/awesome-design-md-55-design-systems-prontos-pro-claude-code|awesome-design-md]] adds that design context is as important as architecture context for good UI.

The business sources extend the same context thesis outward. [[03-wiki/concepts/company-brain|Company Brain]] is the organizational analog of a second brain: a system of record for manuals, prompts, skills, and procedures that agents can consult. [[03-wiki/concepts/agent-friendly-software|Agent-Friendly Software]] suggests that products increasingly need machine-readable interfaces, not only human UIs. [[03-wiki/concepts/ai-native-business-models|AI-Native Business Models]] use AI to deliver outcomes with lower labor cost, while [[03-wiki/concepts/model-aggregator-platforms|Model Aggregator Platforms]] show that model access alone may be less defensible than education, workflow, and distribution.

## Tensions

- Source metadata location: [[03-wiki/sources/build-a-second-brain-that-remembers-everything|Matt Wolfe]] suggests adding YouTube channel metadata to original source frontmatter, while this vault keeps source files unchanged after clipping and records verified `channel` metadata on generated source summary pages. Imported originals are preserved in `01-raw/imports/legacy/raw-originals/`, and processed copies are classified under the relevant `01-raw/` category.
- Speed versus safety: several sources show rapid app generation, but the CRM and full-stack tutorials both warn that authentication, API keys, data privacy, and deployment security still need human review.
- Product versus service: [[03-wiki/sources/6-negocios-de-ia-que-ainda-nao-tem-concorrencia|Deborah Folloni]] argues that AI can make outcome-based services more attractive than SaaS, while the coding sources show how cheap software creation also invites custom internal tools and SaaS challengers.

## Follow-Up Questions

- Should this vault adopt journal and CRM workflows as first-class folders?
- Should there be an automation to process new raw files periodically?
- Which primary sources should be added for Y Combinator requests, OpenRouter pricing, Antigravity docs, Claude Code docs, and `awesome-design-md`?
