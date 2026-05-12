# Relatorio de atualizacao do Second Brain

Data local do vault: 2026-05-11

## O que foi criado

- Estrutura principal numerada:
  - `00-inbox/`
  - `01-raw/`
  - `02-domains/`
  - `03-wiki/`
  - `04-maps/`
  - `05-projects/`
  - `06-outputs/`
  - `07-reviews/`
  - `90-system/`
  - `99-archive/`
- Arquivos raiz:
  - [[index]]
  - [[log]]
- Entrada rapida:
  - [[00-inbox/ideias-soltas]]
  - [[00-inbox/capturas-rapidas]]
- 12 dominios globais em `02-domains/`, cada um com Domain Pack:
  - `_manual.md`
  - `index.md`
  - `log.md`
  - `inbox/`
  - `notes/`
  - `sources/`
  - `concepts/`
  - `entities/`
  - `questions/`
  - `synthesis/`
  - `decisions/`
  - `projects/`
- Camada `03-wiki/` com concepts, entities, sources, comparisons, synthesis, questions, index, log e overview.
- Mapas iniciais em `04-maps/`.
- Projetos iniciais em `05-projects/`:
  - [[05-projects/pulpito-web/index|Pulpito Web]]
  - [[05-projects/second-brain-system/index|Second Brain System]]
  - [[05-projects/roblox-game/index|Roblox Game]]
  - [[05-projects/faculdade-normatic/index|Faculdade Normatic]]
  - [[05-projects/estudos-frontend/index|Estudos Frontend]]
- Subpastas de outputs, revisoes, sistema e arquivo.
- Templates iniciais em `90-system/templates/`.
- Manuais iniciais em `90-system/manuals/`.
- Estrutura de exemplo para espiritualidade, incluindo paginas sobre Davi, Saul, Jonatas, obediencia, arrependimento e lideranca.

## O que foi atualizado

- [[AGENTS]] foi atualizado para descrever a nova arquitetura Second Brain Universal com IA.
- O novo `AGENTS.md` preserva regras importantes da arquitetura antiga Karpathy/LLM Wiki:
  - preservacao de fontes brutas;
  - wiki mantida por IA;
  - logs de ingestao, consulta e lint;
  - cuidado com metadados de canal em fontes do YouTube.
- `log.md` foi criado como log geral do sistema.
- `03-wiki/log.md` foi criado para registrar a migracao da wiki.

## O que ja existia

- `.git/`
- `.obsidian/`
- `raw/`
- `wiki/`
- `AGENTS.md`

## Conteudo preservado

- Nada foi apagado.
- A pasta antiga `raw/` foi mantida.
- A pasta antiga `wiki/` foi mantida.
- Arquivos de `raw/processed/` foram copiados para `01-raw/processed/`.
- Categorias de `wiki/sources/`, `wiki/concepts/`, `wiki/entities/` e `wiki/comparisons/` foram copiadas para `03-wiki/`.
- A sintese antiga `wiki/synthesis.md` foi copiada para `03-wiki/synthesis/sintese-legada-ia-second-brain.md`.

## O que precisa de revisao manual

- Revisar links internos herdados que ainda apontam para `wiki/` em vez de `03-wiki/`.
- Revisar caminhos de fonte herdados que ainda apontam para `raw/` em vez de `01-raw/`.
- Preencher contexto real dos projetos iniciais.
- Decidir se `raw/` e `wiki/` antigos devem continuar como legado permanente ou se o conteudo sera gradualmente consolidado na estrutura numerada.
- Preencher paginas-placeholder de espiritualidade somente com fontes reais.

## Proximos passos recomendados

1. Usar `00-inbox/ideias-soltas.md` e `00-inbox/capturas-rapidas.md` como entrada diaria.
2. Criar uma rotina semanal para processar o inbox.
3. Revisar primeiro o projeto [[05-projects/second-brain-system/index|Second Brain System]].
4. Preencher contexto dos projetos que realmente estiverem ativos.
5. Processar uma primeira nota real de cada dominio principal.
6. Fazer uma revisao semanal usando [[07-reviews/weekly/template-revisao-semanal]].
7. Aos poucos, reconciliar links antigos de `wiki/` com `03-wiki/`.

## Como usar o sistema no dia a dia

Capture rapido:

- Ideias soltas vao para [[00-inbox/ideias-soltas]].
- Pequenas anotacoes vao para [[00-inbox/capturas-rapidas]].
- Arquivos e fontes originais vao para `01-raw/`.

Depois, a IA processa:

- identifica o dominio principal;
- move ou resume o conteudo no Domain Pack correto;
- cria links com conceitos, entidades e projetos;
- atualiza `03-wiki/` quando o conhecimento for reutilizavel;
- atualiza mapas quando uma area crescer;
- registra tudo em logs.

Para consultar:

- Comece por [[index]].
- Use mapas em [[04-maps/index]] para ver o todo.
- Use dominios em [[02-domains/index]] para contexto de vida.
- Use [[03-wiki/index]] para conhecimento conectado.
- Use [[05-projects/index]] para execucao e tarefas.

## Observacao final

Este vault agora esta preparado para funcionar como um sistema em que a pessoa captura sem precisar organizar perfeitamente, e a IA atua como bibliotecaria, analista, arquiteta de conhecimento e mentora para transformar capturas em memoria organizada, conectada e reutilizavel.
