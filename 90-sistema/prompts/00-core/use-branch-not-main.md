# Usar branch em vez da main

## Objetivo

Garantir que tarefas com alteração real rodem fora da main.

## Quando usar

Use antes de executar qualquer prompt que altere conteúdo real, estrutura ou documentação relevante.

## Quando não usar

Não use quando a tarefa for apenas leitura ou explicação.

## Entrada esperada

Tipo de tarefa, descrição curta e data para sugerir nome de branch.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Antes de executar esta tarefa, verifique a branch atual com `git branch --show-current`.
- Se estiver na main, crie uma branch específica para a tarefa.
- Não altere conteúdo real diretamente na main.
- Nome sugerido da branch: `[TIPO]/[DESCRICAO-CURTA]-[DATA]`.
- Depois de criar a branch, execute a tarefa.
- Não faça merge automático.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Garantir que tarefas com alteração real rodem fora da main.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Tipo de tarefa, descrição curta e data para sugerir nome de branch.

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
A tarefa roda em branch apropriada, mantendo a main limpa.
```

## Resultado esperado

A tarefa roda em branch apropriada, mantendo a main limpa.

## Arquivos que podem ser afetados

- Git branch atual
- Arquivos da tarefa solicitada

## Observações

Este prompt não faz merge e não publica alterações sozinho.
