# Gerar relatório de automação

## Objetivo

Gerar resumo de uma automação executada.

## Quando usar

Use após uma rotina ou automação realmente executada.

## Quando não usar

Não use quando nenhum processo foi executado.

## Entrada esperada

Log da execução, arquivos alterados e pendências.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Relatar somente o que aconteceu.
- Não inventar resultados.
- Indicar problemas e próximos passos.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Gerar resumo de uma automação executada.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Log da execução, arquivos alterados e pendências.

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
Relatório de automação claro e verificável.
```

## Resultado esperado

Relatório de automação claro e verificável.

## Arquivos que podem ser afetados

- `06-outputs/reports/`
- `07-reviews/`

## Observações

Este prompt só documenta uma execução real.
