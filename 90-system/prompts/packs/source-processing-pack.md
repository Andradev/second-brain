# Pack de processamento de fontes

## Objetivo

Fluxo composto para classificar e processar fontes brutas preservando originais.

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

1. Usar `00-core/safe-execution-checklist.md`.
2. Usar `11-git-branches/create-feature-branch.md`.
3. Usar `03-raw-sources/classify-raw-inbox.md`.
4. Usar `03-raw-sources/process-specific-source.md`.
5. Usar `03-raw-sources/move-source-to-processed.md`.
6. Usar `14-codex-operations/generate-change-summary.md`.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Executar, somente quando autorizado, o fluxo documentado neste pack.

Fluxo de prompts a considerar:
- 00-core/safe-execution-checklist.md
- 11-git-branches/create-feature-branch.md
- 03-raw-sources/classify-raw-inbox.md
- 03-raw-sources/process-specific-source.md
- 03-raw-sources/move-source-to-processed.md
- 14-codex-operations/generate-change-summary.md

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

Use quando houver fonte real a processar. Não executar automaticamente; apenas documentar o fluxo até que o usuário autorize a execução.
