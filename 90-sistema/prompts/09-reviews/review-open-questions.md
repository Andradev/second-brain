# Revisar perguntas abertas

## Objetivo

Revisar perguntas pendentes em domínios e wiki.

## Quando usar

Use quando perguntas se acumulam ou precisam de decisão.

## Quando não usar

Não use quando não há perguntas reais registradas.

## Entrada esperada

Escopo de perguntas ou domínio.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não inventar respostas.
- Marcar perguntas resolvidas apenas com base real.
- Sugerir próximos passos.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Revisar perguntas pendentes em domínios e wiki.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Escopo de perguntas ou domínio.

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
Lista revisada de perguntas abertas, resolvidas e próximas ações.
```

## Resultado esperado

Lista revisada de perguntas abertas, resolvidas e próximas ações.

## Arquivos que podem ser afetados

- `02-areas/*/questions/`
- `90-sistema/llm-wiki/wiki/questions/`
- `04-revisoes/`

## Observações

Pergunta sem resposta pode continuar aberta.
