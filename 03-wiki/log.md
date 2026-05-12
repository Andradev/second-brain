# Log da wiki

## [2026-05-11] setup | Migracao para 03-wiki

- Criada a estrutura `03-wiki/` com concepts, entities, sources, comparisons, synthesis e questions.
- Copiadas categorias herdadas de `wiki/` para a nova camada numerada sem apagar os arquivos originais.
- Criadas paginas iniciais para conceitos e entidades usados pela nova arquitetura.
- Pendencia: revisar links internos herdados que ainda apontam para `wiki/`.

## [2026-05-11] lint | Limpeza de conteudo simulado

- Removidos conceitos e entidades simulados criados a partir de exemplos.
- Conteudo real da antiga pasta `wiki/` movido para `03-wiki/inbox/legacy-import/wiki/`.
- Duplicatas classificadas removidas quando eram identicas ao legado importado.
- Um arquivo divergente foi movido para `99-archive/review-needed/wiki-classified-leftovers/comparisons/`.
- Regras da wiki atualizadas para impedir conceitos, entidades, sinteses e perguntas vazias.

## [2026-05-12] import | Processamento dos imports legados

- Auditado o lote em `03-wiki/inbox/legacy-import/wiki/`.
- Integrados 10 registros de fonte, 11 conceitos, 17 entidades, 2 comparacoes e 1 sintese.
- Preservados `index.md`, `log.md` e `overview.md` antigos em `03-wiki/imports/legacy/wiki-originals/`.
- Criado manifesto em [[03-wiki/imports/legacy/manifest]].
- Nenhum arquivo foi movido para `review-needed` nesta rodada.
