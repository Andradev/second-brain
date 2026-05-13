# Pack de memórias contextuais

## Objetivo

Fluxo para consultar, sugerir, criar ou atualizar memórias contextuais com segurança.

## Quando usar

Use quando o fluxo composto for mais adequado do que um prompt isolado.

## Quando não usar

Não use quando a tarefa for simples, quando faltar confirmação humana ou quando o objetivo for executar todos os passos automaticamente.

## Entrada esperada

Objetivo do fluxo, escopo, data ou período, e confirmação de quais etapas devem ser executadas.

## Regras importantes

- Este pack é documentação de fluxo, não execução automática.
- Não executar todos os prompts apenas por estarem listados.
- Não criar conteúdo simulado.
- Não apagar conteúdo real.
- Usar branch separada quando houver alteração real.
- Parar e pedir confirmação se o escopo crescer.

## Fluxo

1. Usar `06-context-memory/consult-context-memories.md`.
2. Usar `06-context-memory/suggest-context-memory.md`.
3. Usar `06-context-memory/create-context-memory.md`.
4. Usar `06-context-memory/update-context-memory.md`.
5. Usar `06-context-memory/archive-context-memory.md`.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Executar, somente quando autorizado, o fluxo documentado neste pack.

Fluxo de prompts a considerar:
- 06-context-memory/consult-context-memories.md
- 06-context-memory/suggest-context-memory.md
- 06-context-memory/create-context-memory.md
- 06-context-memory/update-context-memory.md
- 06-context-memory/archive-context-memory.md

Regras:
1. Não execute automaticamente todos os prompts listados.
2. Confirme o escopo antes de cada etapa que altere conteúdo real.
3. Não criar conteúdo simulado.
4. Não apagar conteúdo real.
5. Usar branch separada quando houver alteração real.
6. Não fazer merge automático.

Resultado esperado:
Fluxo conduzido em etapas claras, com alterações limitadas ao escopo autorizado.
```

## Resultado esperado

Uma sequência segura de prompts, aplicada apenas nas etapas confirmadas pelo usuário.

## Arquivos que podem ser afetados

Depende dos prompts escolhidos no fluxo. Consulte cada prompt antes de executar.

## Observações

Use quando o assunto envolver lembretes recorrentes. Não executar automaticamente; apenas documentar o fluxo até que o usuário autorize a execução.
