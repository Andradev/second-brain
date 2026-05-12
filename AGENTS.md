# AGENTS.md

## Proposito do Second Brain

Este vault e um Second Brain Universal com IA.

Ele existe para capturar, organizar, conectar e sintetizar o conhecimento pessoal do usuario ao longo da vida.

O sistema deve reunir notas soltas, estudos, aulas, videos, devocionais, diario pessoal, trabalho, faculdade, projetos, ideias, decisoes e fontes brutas.

A IA deve transformar essas entradas em conhecimento estruturado, conectado e reutilizavel.

## Principios centrais

1. O usuario captura de forma simples.
2. A IA organiza de forma estruturada.
3. Fontes originais devem ser preservadas.
4. O conhecimento deve ser conectado com links internos.
5. A wiki deve ser viva e atualizada.
6. Toda area importante deve ter manual proprio.
7. Toda alteracao relevante deve ser registrada em log.md.
8. O sistema deve crescer sem virar bagunca.
9. O vault deve favorecer clareza, reutilizacao e revisao.
10. A IA deve criar contexto, nao apenas armazenar texto.

## Estrutura principal

- `00-inbox/`: entrada livre e rapida para capturas ainda caoticas.
- `01-raw/`: fontes brutas e originais.
- `02-domains/`: grandes areas da vida humana.
- `03-wiki/`: conhecimento estruturado e conectado.
- `04-maps/`: mapas de navegacao e visao geral.
- `05-projects/`: projetos ativos.
- `06-outputs/`: saidas finais geradas pela IA.
- `07-reviews/`: revisoes periodicas.
- `90-system/`: sistema interno, manuais, templates e regras.
- `99-archive/`: conteudo arquivado, antigo ou substituido.

## Compatibilidade com estrutura legada

Este vault nasceu com a estrutura Karpathy/LLM Wiki em `raw/` e `wiki/`.

- `raw/` e `wiki/` devem ser preservados.
- Nao apagar, renomear ou mover arquivos dessas pastas sem pedido explicito do usuario.
- Novos fluxos devem preferir `01-raw/` e `03-wiki/`.
- Quando necessario, use os conteudos antigos como fontes de contexto e copie ou referencie o que for util para a nova arquitetura.
- Para consultas, leia primeiro `index.md`; se a pergunta envolver conhecimento ja processado, consulte tambem `03-wiki/index.md` e, quando relevante, a antiga `wiki/index.md`.

## Fluxo profissional

O fluxo principal do sistema e:

Capturar -> Classificar -> Processar -> Conectar -> Sintetizar -> Revisar -> Reutilizar

1. Capturar: o usuario joga uma ideia em `00-inbox/`.
2. Classificar: a IA identifica dominio principal, dominios secundarios, conceitos, entidades e projetos relacionados.
3. Processar: a IA cria uma nota limpa no local correto.
4. Conectar: a IA cria links internos com conceitos, entidades, projetos, decisoes e fontes.
5. Sintetizar: a IA atualiza paginas de sintese quando um tema se torna recorrente.
6. Revisar: a IA identifica padroes, lacunas, notas orfas e proximos passos.
7. Reutilizar: o usuario consulta o proprio conhecimento acumulado para estudar, decidir e construir.

## Regras de seguranca

1. Nao apagar nenhum arquivo existente.
2. Nao sobrescrever arquivos existentes sem preservar ou mesclar o conteudo util.
3. Se uma pasta ja existir, manter a pasta e complementar a estrutura.
4. Fontes brutas em `01-raw/` sao fontes originais e nao devem ser reescritas.
5. Se houver duvida sobre classificacao, manter em `00-inbox/para-processar/` e registrar a duvida.
6. Se uma nota tocar em mais de uma area, escolher uma area principal e criar links cruzados.

## Regras de processamento

Ao processar uma nova nota:

1. Ler o conteudo.
2. Identificar o tipo da nota.
3. Identificar o dominio principal.
4. Identificar dominios secundarios.
5. Identificar conceitos.
6. Identificar entidades.
7. Identificar projetos relacionados.
8. Criar ou atualizar nota processada no local correto.
9. Criar links internos com `[[wikilinks]]`.
10. Atualizar `index.md` da area.
11. Atualizar `log.md` da area.
12. Atualizar `03-wiki/` quando houver conceito ou entidade relevante.
13. Atualizar `synthesis/` quando o tema for recorrente.
14. Registrar duvidas em `questions/`.
15. Preservar a fonte original.

## Regras para classificacao

- Pensamento rapido: `00-inbox/`.
- Fonte original: `01-raw/`.
- Area da vida: `02-domains/`.
- Conceito reutilizavel: `03-wiki/concepts/`.
- Pessoa, personagem, empresa, ferramenta, lugar ou projeto: `03-wiki/entities/`.
- Visao geral: `04-maps/`.
- Projeto ativo: `05-projects/`.
- Saida final: `06-outputs/`.
- Revisao: `07-reviews/`.
- Conteudo antigo: `99-archive/`.

## Regras de links

Use links internos no formato `[[nome-do-conceito]]`.

Sempre que possivel, conecte:

- Nota com conceito.
- Conceito com entidade.
- Entidade com projeto.
- Projeto com decisao.
- Fonte com sintese.
- Diario com aprendizado.
- Estudo com projeto pratico.
- Devocional com personagem biblico.
- Trabalho com regra de negocio.
- Ideia com possivel projeto.

Exemplos:

- Uma nota sobre Davi deve conectar `[[davi]]`, `[[obediencia]]`, `[[lideranca]]`, `[[arrependimento]]` e estudos biblicos relacionados.
- Uma nota sobre React deve conectar `[[react]]`, `[[javascript]]`, `[[typescript]]`, `[[frontend]]` e projetos que usam React.
- Uma nota sobre Pulpito Web deve conectar `[[pulpito-web]]`, `[[laravel]]`, `[[mysql]]`, `[[api-rest]]` e `[[requisitos-de-software]]`.

## Regras de escrita

- Escrever em portugues do Brasil.
- Usar Markdown limpo.
- Usar titulos claros.
- Usar listas quando ajudar.
- Usar nomes de arquivos em kebab-case.
- Evitar duplicidade.
- Ser claro e pratico.
- Nao inventar informacoes que nao estao nas fontes.
- Quando fizer inferencia, deixar claro.

## Frontmatter padrao

Todas as notas processadas devem usar este frontmatter:

```yaml
---
title: ""
type: "note"
domain: ""
status: "processed"
created: YYYY-MM-DD
updated: YYYY-MM-DD
source_type: ""
related: []
tags: []
---
```

## Tipos possiveis

`type` pode ser:

- `note`
- `source`
- `concept`
- `entity`
- `synthesis`
- `question`
- `decision`
- `project`
- `review`
- `output`
- `manual`

`status` pode ser:

- `inbox`
- `processing`
- `processed`
- `reviewed`
- `archived`

`source_type` pode ser:

- `journal`
- `video`
- `article`
- `book`
- `class`
- `work`
- `bible`
- `meeting`
- `idea`
- `conversation`
- `unknown`

## Logs

Sempre que processar algo, registrar no `log.md` relevante:

```md
## YYYY-MM-DD

- Processado: [[arquivo-original]]
- Criado: [[nova-nota]]
- Atualizado: [[conceito]], [[entidade]], [[sintese]]
- Observacoes:
- Pendencias:
```

O log antigo da wiki usa tambem o formato:

```md
## [YYYY-MM-DD] tipo | Titulo
```

Esse formato continua valido para paginas herdadas da LLM Wiki, especialmente em `wiki/log.md` e `03-wiki/log.md`.

## Domain Pack

Cada dominio em `02-domains/` deve conter:

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

Antes de processar uma nota dentro de um dominio, leia o `_manual.md` daquele dominio.

## Regras para 01-raw

- Nunca reescrever a fonte original.
- Quando processar uma fonte, criar nota limpa em `02-domains/` ou `03-wiki/`.
- Criar links da nota processada de volta para a fonte original.
- Se uma fonte gerar varios conceitos, criar ou atualizar paginas em `03-wiki/concepts/`.
- Se uma fonte mencionar pessoas, personagens, empresas, ferramentas ou projetos, criar ou atualizar paginas em `03-wiki/entities/`.
- Se uma fonte for muito importante, criar ou atualizar uma sintese em `03-wiki/synthesis/`.

Para videos do YouTube salvos por Web Clipper, paginas de resumo de fonte devem incluir frontmatter com `channel` quando o canal puder ser verificado. Se nao puder, usar `channel: "unknown"` e registrar a duvida.

## Regras para consultas

Ao responder uma pergunta:

1. Ler `index.md` primeiro.
2. Ler paginas relevantes em `02-domains/`, `03-wiki/`, `04-maps/` e `05-projects/`.
3. Consultar fontes em `01-raw/` ou `raw/` quando a resposta depender da origem.
4. Responder com citacoes para paginas do vault e caminhos de fontes quando disponiveis.
5. Se a resposta tiver valor duravel, registrar em uma pagina adequada, atualizar indice e log.

## Regras para lint

Quando o usuario pedir uma revisao de saude do wiki:

1. Procurar contradicoes.
2. Procurar claims stale ou sem fonte.
3. Procurar paginas orfas.
4. Procurar referencias cruzadas ausentes.
5. Procurar conceitos importantes sem pagina.
6. Procurar dados faltantes.
7. Fazer manutencoes diretas quando forem seguras.
8. Registrar no log.

## Quando tiver duvida

Se a IA nao souber onde colocar uma nota:

1. Nao inventar.
2. Colocar em `00-inbox/para-processar/`.
3. Criar observacao no `log.md`.
4. Sugerir 2 ou 3 classificacoes provaveis quando isso ajudar.
