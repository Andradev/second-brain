# Raw

Esta pasta guarda fontes brutas e originais.

## Entrada geral

- `inbox/`: fontes novas ainda sem categoria clara.

## Categorias

Cada categoria usa a mesma estrutura:

- `inbox/`: fontes ainda nao processadas.
- `processed/`: fontes ja processadas pela IA.
- `archive/`: fontes antigas, duplicadas ou arquivadas.

Categorias:

- `articles/`
- `videos/`
- `books/`
- `bible/`
- `classes/`
- `work/`
- `meetings/`
- `images/`
- `assets/`

## Imports legados

- `imports/legacy/raw-originals/`: originais preservados de importacoes antigas.
- `imports/legacy/manifest.md`: auditoria dos arquivos importados.
- `imports/legacy/review-needed/`: fontes antigas que precisam de revisao manual.
- Fontes classificadas saem de `imports/legacy/` para o `processed/` da categoria correta quando ja foram processadas com seguranca.

## Regras

- Nao usar `01-raw/processed/` global.
- Nao reescrever fonte original.
- Criar notas processadas em `02-domains/` ou `03-wiki/` somente a partir de conteudo real.
- Registrar caminhos de fonte nas notas derivadas.

## Manual de uso

- [[01-raw/README|Manual de uso]]
