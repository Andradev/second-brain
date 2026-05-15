# Manual: Domains

## Proposito

`02-areas/` representa as grandes areas da vida.

Dominios guardam contexto de vida. A wiki guarda conhecimento conectado.

## Regra contra conteudo simulado

Conteudo dentro de dominio so deve ser criado a partir de:

1. Nota real do usuario.
2. Fonte real do usuario.
3. Conteudo real ja existente no vault.
4. Pedido explicito do usuario.

Exemplos em manuais nao devem virar arquivos reais.

## Domain Pack

Cada dominio deve seguir o Domain Pack:

- `_manual.md`
- `index.md`
- `log.md`
- `inbox/`
- `notes/`
- `memory/`
- `sources/`
- `concepts/`
- `entities/`
- `questions/`
- `synthesis/`
- `decisions/`
- `projects/`

A pasta `memory/` guarda memorias recorrentes daquele dominio. Sao lembretes persistentes que a IA deve considerar quando o assunto aparecer novamente.

## Como processar

Antes de mexer em um dominio, ler o `_manual.md` local.

Sempre atualizar o `index.md` e o `log.md` quando algo relevante for criado ou processado.

Nao criar notas, conceitos, entidades, fontes, sinteses, decisoes, projetos ou memorias simulados.
