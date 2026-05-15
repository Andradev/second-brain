# Extrair ações de uma nota

## Objetivo

Identificar tarefas, decisões pendentes e próximos passos em uma nota real do usuário.

## Quando usar

Use quando uma nota contém coisas a fazer misturadas com reflexão.

## Quando não usar

Não use quando a nota for apenas material de referência sem ação.

## Entrada esperada

Nota real do usuário e destino desejado para as ações.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não inventar tarefas.
- Separar ação explícita de sugestão inferida.
- Não criar projeto ativo sem confirmação.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Identificar tarefas, decisões pendentes e próximos passos em uma nota real do usuário.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Nota real do usuário e destino desejado para as ações.

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
Lista de ações extraídas, com pendências e dúvidas.
```

## Resultado esperado

Lista de ações extraídas, com pendências e dúvidas.

## Arquivos que podem ser afetados

- `00-inbox/`
- `03-projetos/inbox/`
- `90-sistema/llm-wiki/wiki/questions/`

## Observações

Ações inferidas devem ser marcadas como inferência.
