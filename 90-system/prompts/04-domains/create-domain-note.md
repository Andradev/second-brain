# Criar nota de domínio

## Objetivo

Criar uma nota processada em um domínio a partir de conteúdo real.

## Quando usar

Use quando houver nota, fonte ou pedido explícito do usuário.

## Quando não usar

Não use quando a informação vier só de exemplo conceitual.

## Entrada esperada

Conteúdo real, domínio principal e fonte, se houver.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Usar frontmatter padrão.
- Criar wikilinks apenas para conhecimento real.
- Atualizar log do domínio.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Criar uma nota processada em um domínio a partir de conteúdo real.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Conteúdo real, domínio principal e fonte, se houver.

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
Nota processada criada em `notes/` ou área adequada do domínio.
```

## Resultado esperado

Nota processada criada em `notes/` ou área adequada do domínio.

## Arquivos que podem ser afetados

- `02-domains/[domínio]/notes/`
- `02-domains/[domínio]/log.md`

## Observações

Se a classificação for incerta, deixe pendência clara.
