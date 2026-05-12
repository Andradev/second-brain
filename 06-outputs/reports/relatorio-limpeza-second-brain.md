# Relatorio de limpeza do Second Brain

## Objetivo

Limpar conteudo simulado, consolidar estruturas duplicadas e ajustar o fluxo de fontes brutas.

## Arquivos simulados removidos

- `03-wiki/concepts/aprendizagem-pratica.md`
- `03-wiki/concepts/arrependimento.md`
- `03-wiki/concepts/lideranca.md`
- `03-wiki/concepts/obediencia.md`
- `03-wiki/entities/davi.md`
- `03-wiki/entities/jonatas.md`
- `03-wiki/entities/pulpito-web.md`
- `03-wiki/entities/saul.md`
- `02-domains/09-spirituality-values/concepts/arrependimento.md`
- `02-domains/09-spirituality-values/concepts/lideranca.md`
- `02-domains/09-spirituality-values/concepts/obediencia.md`
- `02-domains/09-spirituality-values/entities/davi.md`
- `02-domains/09-spirituality-values/entities/jonatas.md`
- `02-domains/09-spirituality-values/entities/saul.md`
- `02-domains/09-spirituality-values/notes/devocional-2026-05-11.md`
- `02-domains/09-spirituality-values/notes/reflexao-sobre-davi.md`
- `02-domains/09-spirituality-values/questions/o-que-deus-ensina-com-a-historia-de-davi.md`
- `02-domains/09-spirituality-values/sources/estudo-biblico-1-samuel.md`
- `02-domains/09-spirituality-values/sources/pregacao-sobre-davi.md`
- `02-domains/09-spirituality-values/synthesis/o-que-ja-aprendi-sobre-davi.md`
- `02-domains/09-spirituality-values/decisions/decisoes-espirituais.md`
- `02-domains/09-spirituality-values/projects/estudos-biblicos/`

## Projetos simulados removidos

- `05-projects/estudos-frontend/`
- `05-projects/faculdade-normatic/`
- `05-projects/pulpito-web/`
- `05-projects/roblox-game/`
- `05-projects/second-brain-system/`

## Estruturas consolidadas

- A pasta antiga `raw/` foi movida para `01-raw/inbox/legacy-import/raw/`.
- A pasta antiga `wiki/` foi movida para `03-wiki/inbox/legacy-import/wiki/`.
- As duplicatas criadas anteriormente em `01-raw/processed/` foram removidas quando eram identicas ao legado importado.
- As duplicatas criadas anteriormente em `03-wiki/sources/`, `03-wiki/concepts/`, `03-wiki/entities/`, `03-wiki/comparisons/` e `03-wiki/synthesis/` foram removidas quando eram identicas ao legado importado.
- A regra final e: fontes brutas ficam em `01-raw/` e wiki estruturada fica em `03-wiki/`.

## Nova organizacao de 01-raw

`01-raw/` agora tem uma entrada geral de fontes:

- `01-raw/inbox/`

Cada categoria de fonte tem:

- `inbox/`
- `processed/`
- `archive/`

Categorias criadas:

- `articles/`
- `videos/`
- `books/`
- `bible/`
- `classes/`
- `work/`
- `meetings/`
- `images/`
- `assets/`

Nao existe mais `01-raw/processed/` global.

## Arquivos movidos para revisao manual

- `99-archive/review-needed/wiki-classified-leftovers/comparisons/adapta-myhub-inner-ai-alternatives.md`

Motivo: o arquivo tinha o mesmo nome de um item importado do legado, mas o hash nao era identico. Foi preservado para revisao manual em vez de apagado.

## Regras adicionadas ao AGENTS.md

- A IA nunca deve criar conteudo ficticio, simulado ou baseado apenas em exemplos de documentacao.
- Exemplos em manuais, prompts ou templates sao apenas exemplos conceituais.
- Notas, conceitos, entidades, projetos, fontes, perguntas, decisoes e sinteses so podem ser criados a partir de conteudo real, conteudo existente ou pedido explicito do usuario.
- Projetos nao devem ser criados automaticamente.
- `01-raw/processed/` global nao deve ser usado.
- `raw/` e `wiki/` nao devem existir soltos na raiz.
- Se houver duvida se algo e real, mover para `99-archive/review-needed/`.

## Proximos passos

1. Jogar fontes novas em `01-raw/inbox/`.
2. Jogar ideias soltas em `00-inbox/`.
3. Pedir para a IA processar fontes especificas.
4. Criar projetos somente quando voce pedir ou confirmar.
5. Criar paginas de wiki somente a partir de conteudo real.
6. Revisar o legado em `01-raw/inbox/legacy-import/raw/` e `03-wiki/inbox/legacy-import/wiki/` quando quiser consolidar o conhecimento antigo.
