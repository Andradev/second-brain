# Checklist de execução segura

## Objetivo

Verificar branch, git status, escopo, riscos e possibilidade de apagar conteúdo real antes de executar uma tarefa.

## Quando usar

Use antes de operações que movem, alteram, criam ou arquivam arquivos.

## Quando não usar

Não use para perguntas puramente conceituais que não alteram arquivos.

## Entrada esperada

Descrição da tarefa, escopo pretendido e pastas possivelmente afetadas.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Verificar branch atual.
- Verificar git status.
- Identificar risco de perda de conteúdo.
- Parar e pedir confirmação se houver risco alto.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Verificar branch, git status, escopo, riscos e possibilidade de apagar conteúdo real antes de executar uma tarefa.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Descrição da tarefa, escopo pretendido e pastas possivelmente afetadas.

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
Checklist concluído antes de qualquer alteração operacional.
```

## Resultado esperado

Checklist concluído antes de qualquer alteração operacional.

## Arquivos que podem ser afetados

- Pode apenas consultar git e arquivos relevantes
- Não deve alterar conteúdo sozinho

## Observações

Use este prompt como primeira etapa de fluxos sensíveis.
