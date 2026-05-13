# Atualizar contexto do projeto

## Objetivo

Atualizar contexto de projeto com informações reais novas.

## Quando usar

Use quando houver nova nota, decisão ou fonte relacionada.

## Quando não usar

Não use quando a informação for suposição não confirmada.

## Entrada esperada

Projeto, nova informação e origem.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Preservar histórico útil.
- Separar fato de hipótese.
- Linkar fontes.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Atualizar contexto de projeto com informações reais novas.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Projeto, nova informação e origem.

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
Contexto do projeto atualizado e rastreável.
```

## Resultado esperado

Contexto do projeto atualizado e rastreável.

## Arquivos que podem ser afetados

- `05-projects/active/[projeto]/`

## Observações

Não reescrever estratégia sem motivo claro.
