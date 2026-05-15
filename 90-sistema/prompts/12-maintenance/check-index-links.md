# Verificar links de índices

## Objetivo

Conferir se índices e READMEs apontam para arquivos existentes.

## Quando usar

Use quando links parecem quebrados ou após reorganização.

## Quando não usar

Não use quando não houve mudança de links.

## Entrada esperada

Índices a verificar.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não criar páginas faltantes só para satisfazer link.
- Corrigir links óbvios quando autorizado.
- Listar links quebrados.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Conferir se índices e READMEs apontam para arquivos existentes.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Índices a verificar.

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
6. Se houver dúvida relevante, pedir confirmação ou mover para 99-arquivo/revisar.
7. Não fazer merge automático.

Resultado esperado:
Índices com problemas identificados ou corrigidos.
```

## Resultado esperado

Índices com problemas identificados ou corrigidos.

## Arquivos que podem ser afetados

- `README.md`
- `index.md`
- `90-sistema/llm-wiki/wiki/`
- `90-sistema/`

## Observações

Link quebrado pode indicar conteúdo não criado de propósito.
