# Antigravity And Claude Code Roles

Comparison of how [[wiki/sources/antigravity-com-claude-code-e-absurdo-crie-um-crm-completo|Antigravity com Claude Code e Absurdo]] divides work between Google Antigravity and Claude Code.

| Tool | Role In The Workflow | Best Used For | Watchouts |
| --- | --- | --- | --- |
| [[wiki/entities/google-antigravity|Google Antigravity]] | Visual workspace and project cockpit | File navigation, visual planning, UI generation with Gemini, prompt iteration | Built-in model quotas and changing model availability |
| [[wiki/entities/claude-code|Claude Code]] | Implementation agent and code executor | Backend logic, data behavior, complex fixes, structured code changes | Requires permissions, review, and verification |
| Human operator | Product owner and reviewer | Choosing references, writing prompts, testing behavior, accepting changes | Must still audit security before deployment |

## Current Takeaway

The source argues for a division of labor: use the visual AI IDE to stay oriented and generate a polished first pass, then use the stronger coding agent for deeper behavior and backend work. This complements [[wiki/concepts/spec-driven-agentic-development|Spec-Driven Agentic Development]], which adds more formal context and feature-spec discipline.

## Supporting Sources

- [[wiki/sources/antigravity-com-claude-code-e-absurdo-crie-um-crm-completo|Antigravity com Claude Code e Absurdo]]
- [[wiki/sources/crie-um-agente-de-ia-no-whatsapp-com-crm|Crie um Agente de IA no WhatsApp com CRM]]

## Related Pages

- [[wiki/concepts/agentic-coding-workflow|Agentic Coding Workflow]]
- [[wiki/entities/google-antigravity|Google Antigravity]]
- [[wiki/entities/claude-code|Claude Code]]

## Open Questions

- Which parts of this workflow translate cleanly to Codex inside this vault?
