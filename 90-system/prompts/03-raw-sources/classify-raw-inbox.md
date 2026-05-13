# Classificar raw inbox

## Objetivo

Classificar fontes novas em `01-raw/inbox/` para a categoria correta.

## Quando usar

Use quando houver fontes brutas sem categoria clara.

## Quando não usar

Não use quando a fonte já estiver em categoria correta e pronta para processamento.

## Entrada esperada

Arquivos em `01-raw/inbox/` ou lista de fontes.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não editar a fonte original.
- Mover apenas para inbox/archive da categoria correta.
- Não criar nota processada nessa etapa, salvo pedido explícito.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Classificar fontes novas em `01-raw/inbox/` para a categoria correta.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Arquivos em `01-raw/inbox/` ou lista de fontes.

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
Fontes classificadas por tipo com dúvidas preservadas.
```

## Resultado esperado

Fontes classificadas por tipo com dúvidas preservadas.

## Arquivos que podem ser afetados

- `01-raw/inbox/`
- `01-raw/articles/inbox/`
- `01-raw/videos/inbox/`
- `01-raw/classes/inbox/`

## Observações

Classificação é diferente de processamento.
