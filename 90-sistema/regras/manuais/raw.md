# Manual: Fontes

## Proposito

`01-fontes/` guarda fontes brutas e originais.

Fontes brutas entram aqui antes de virarem notas organizadas, conceitos ou sinteses.

## Estrutura simples

- `inbox/`: fonte nova ou pendente.
- `processadas/`: fonte ja usada pela IA.
- `arquivadas/`: fonte antiga, duplicada ou sem uso agora.

Nao criar subpastas visiveis por tipo de fonte dentro de `01-fontes/`.

A classificacao detalhada deve ser feita por titulo, metadados, tags, links internos ou anotacao da IA.

## Fluxo

1. Fonte nova entra em `01-fontes/inbox/`.
2. A IA identifica tipo, assunto, area provavel e relacoes.
3. Se houver pedido de processamento, a IA cria nota organizada em `02-areas/`.
4. Se houver conhecimento recorrente, a IA atualiza `90-sistema/llm-wiki/wiki/`.
5. A fonte original vai para `01-fontes/processadas/`.

## Arquivamento

Se uma fonte for duplicada, antiga ou nao for util agora, mover para `01-fontes/arquivadas/`.

Se houver duvida sobre a origem ou classificacao, manter em `01-fontes/inbox/` ou mover para `99-arquivo/revisar/`.

## Regras

- Preservar a fonte original.
- Nao reescrever fonte bruta.
- Nao apagar fontes reais sem pedido explicito.
- Nao criar fonte simulada.
- Nao processar fonte sem base real.
