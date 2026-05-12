# Supabase

Backend platform used as Postgres database, authentication provider, and integration target in the WhatsApp AI CRM workflow.

## Current Synthesis

Supabase stores lead and chat-history data for the WhatsApp CRM tutorial. It also provides authentication for the CRM interface and can be connected to Antigravity through MCP so the AI development environment can inspect and build against the database.

## Supporting Sources

- [[03-wiki/sources/crie-um-agente-de-ia-no-whatsapp-com-crm|Crie um Agente de IA no WhatsApp com CRM]]

## Related Pages

- [[03-wiki/entities/n8n|n8n]]
- [[03-wiki/entities/google-antigravity|Google Antigravity]]
- [[03-wiki/concepts/ai-agent-crm|AI Agent CRM]]

## Open Questions

- What row-level security and credential practices should be required before production deployment?
