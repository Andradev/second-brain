# Criar nota de área

## Objetivo

Criar uma nota processada em uma área a partir de conteúdo real.

## Quando usar

Use quando houver nota, fonte ou pedido explícito do usuário.

## Quando não usar

Não use quando a informação vier só de exemplo conceitual.

## Entrada esperada

Conteúdo real, área principal e fonte, se houver.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Usar frontmatter padrão.
- Criar wikilinks apenas para conhecimento real.
- Atualizar log da área.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Criar uma nota processada em uma área a partir de conteúdo real.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Conteúdo real, área principal e fonte, se houver.

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
Nota processada criada na área adequada.
```

## Resultado esperado

Nota processada criada na área adequada.

## Arquivos que podem ser afetados

- `02-areas/[area-principal]/`
- `02-areas/[area-principal]/README.md`

## Observações

Se a classificação for incerta, deixe pendência clara.
