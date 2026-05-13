# Atualizar AGENTS.md

## Objetivo

Atualizar regras de agente com cuidado e sem quebrar princípios existentes.

## Quando usar

Use quando o usuário pedir mudança em `AGENTS.md`.

## Quando não usar

Não use quando a regra pertence a manual ou prompt, não ao agente global.

## Entrada esperada

Texto da regra e motivo.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Preservar regras existentes.
- Não contradizer segurança central.
- Explicar mudança.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Atualizar regras de agente com cuidado e sem quebrar princípios existentes.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Texto da regra e motivo.

Tarefa:
1. Verifique o escopo solicitado.
2. Consulte regras, manuais e memórias contextuais relevantes quando aplicável.
3. Execute apenas a tarefa descrita neste prompt.
4. Preserve conteúdo real e registre dúvidas quando houver incerteza.
5. Ao final, informe o que foi criado, atualizado, movido ou deixado pendente.

Regras:
1. Não criar conteúdo simulado.
2. Não inventar informações.
3. Não apagar conteúdo real.
4. Respeitar a estrutura do Second Brain.
5. Registrar alterações quando necessário.
6. Se houver dúvida relevante, pedir confirmação ou mover para review-needed.
7. Não fazer merge automático.

Resultado esperado:
`AGENTS.md` atualizado com seção ou ajuste claro.
```

## Resultado esperado

`AGENTS.md` atualizado com seção ou ajuste claro.

## Arquivos que podem ser afetados

- `AGENTS.md`

## Observações

AGENTS.md é regra central; edite com parcimônia.
