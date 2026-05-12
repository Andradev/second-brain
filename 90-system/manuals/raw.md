# Manual: Raw

## Proposito

`01-raw/` guarda fontes brutas e originais.

Fontes brutas entram aqui antes de virarem conhecimento processado.

## Estrutura

- `inbox/`: entrada geral de fontes ainda sem categoria clara.
- `articles/`
- `videos/`
- `books/`
- `bible/`
- `classes/`
- `work/`
- `meetings/`
- `images/`
- `assets/`

Cada categoria deve conter:

- `inbox/`
- `processed/`
- `archive/`

## Fluxo de fontes brutas

### 1. Captura inicial

Toda fonte nova entra primeiro em `01-raw/inbox/` ou diretamente no inbox da categoria, se a categoria ja for clara.

Exemplos conceituais:

- Artigo novo: `01-raw/articles/inbox/`
- Video novo: `01-raw/videos/inbox/`
- Aula nova: `01-raw/classes/inbox/`
- Fonte de trabalho: `01-raw/work/inbox/`
- Fonte biblica: `01-raw/bible/inbox/`
- Reuniao: `01-raw/meetings/inbox/`

Esses exemplos nao autorizam a criacao de arquivos reais.

### 2. Classificacao

A IA identifica o tipo da fonte e move para o inbox da categoria correta.

### 3. Processamento

Ao processar uma fonte, a IA deve:

1. Ler a fonte bruta.
2. Criar nota processada no dominio correto em `02-domains/`, se houver conteudo real.
3. Criar ou atualizar conceitos em `03-wiki/concepts/`, somente se vierem da fonte.
4. Criar ou atualizar entidades em `03-wiki/entities/`, somente se vierem da fonte.
5. Criar ou atualizar sinteses em `03-wiki/synthesis/`, somente se houver conteudo real suficiente.
6. Criar links internos.
7. Atualizar index e log.
8. Registrar a fonte usada.
9. Mover a fonte bruta para `processed/` da propria categoria.

### 4. Arquivamento

Se uma fonte for duplicada, antiga ou nao for util agora, mover para `archive/` da categoria correspondente.

## Regras

- Nao usar `01-raw/processed/` global.
- Nao reescrever fonte bruta.
- Nao apagar fontes reais sem pedido explicito.
- Nao criar fonte simulada.
- Se houver duvida sobre origem ou classificacao, mover para `99-archive/review-needed/`.
