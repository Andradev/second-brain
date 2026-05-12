---
source_path: "raw/processed/Crie um Agente de IA no WhatsApp com CRM (Guia Completo n8n + Antigravity).md"
source_url: "https://www.youtube.com/watch?v=Jvq47ed-fm4"
source_type: "youtube"
channel: "Felipe Borges - Fala IA!"
published: 2026-03-09
processed: 2026-05-11
---

# Crie um Agente de IA no WhatsApp com CRM

Source path: `raw/processed/Crie um Agente de IA no WhatsApp com CRM (Guia Completo n8n + Antigravity).md`

Processed date: 2026-05-11

## Short Summary

Felipe Borges gives a long, implementation-oriented walkthrough for building a WhatsApp AI agent connected to a visual CRM. The system uses n8n for automation, Z-API for WhatsApp integration, Supabase/Postgres for lead and chat history storage, and Google Antigravity to build the CRM interface.

## Key Claims Or Observations

- A WhatsApp bot becomes more valuable when paired with a CRM that exposes conversations, leads, and history to owners, partners, and developers.
- The n8n flow receives WhatsApp messages through a webhook, filters activation conditions, normalizes lead data, sends messages to an AI model, and returns responses through Z-API.
- Supabase stores leads and chat history; phone number/session ID is used as a shared key to relate lead records to conversations.
- Antigravity can connect to Supabase through MCP, generate a CRM from a provided Markdown replication kit and design reference, then iterate UI behavior through prompts.
- Authentication is required so only approved users can access conversation data.
- The tutorial repeatedly tests each integration step and fixes mismatched credentials, missing message fields, and timestamp formatting.

## Relevant Entities

- [[wiki/entities/felipe-borges-fala-ia|Felipe Borges - Fala IA!]]
- [[wiki/entities/n8n|n8n]]
- [[wiki/entities/supabase|Supabase]]
- [[wiki/entities/google-antigravity|Google Antigravity]]
- WhatsApp
- Z-API

## Relevant Concepts

- [[wiki/concepts/ai-agent-crm|AI Agent CRM]]
- [[wiki/concepts/agentic-coding-workflow|Agentic Coding Workflow]]
- [[wiki/concepts/company-brain|Company Brain]]

## Contradictions, Tensions, Or Updates

- The source treats AI automation as a client-service asset, reinforcing the [[wiki/concepts/ai-native-business-models|AI-Native Business Models]] idea that better packaging and visibility can justify higher project value.
- It also raises data-access and authentication concerns, because CRM visibility over WhatsApp conversations creates sensitive-data exposure.

## Open Questions

- Which WhatsApp API provider should be preferred for a production version?
- What security checklist should be added before deploying a client CRM with real messages?
