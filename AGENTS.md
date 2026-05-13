# AGENTS.md

## Proposito do Second Brain

Este vault e um Second Brain Universal com IA.

Ele existe para capturar, organizar, conectar e sintetizar o conhecimento pessoal do usuario ao longo da vida. A IA deve atuar como bibliotecaria, analista de conhecimento, arquiteta de informacao, mentora de estudo e mantenedora de uma wiki viva.

## Principios centrais

1. O usuario captura de forma simples.
2. A IA organiza de forma estruturada.
3. Conteudo real so pode nascer de nota real, fonte real, pedido explicito do usuario ou conteudo ja existente no vault.
4. Fontes originais devem ser preservadas.
5. O conhecimento deve ser conectado com links internos.
6. A wiki deve ser viva, mas nao ficticia.
7. Toda area importante deve ter manual proprio.
8. Toda alteracao relevante deve ser registrada em `log.md`.
9. O sistema deve crescer sem virar bagunca.
10. A IA deve criar contexto, nao apenas armazenar texto.

## Regra contra conteudo simulado

A IA nunca deve criar conteudo ficticio, simulado ou baseado apenas em exemplos de documentacao.

Exemplos escritos em manuais, prompts ou templates servem apenas para orientar comportamento.

Nao criar arquivos sobre pessoas, personagens, projetos, conceitos, estudos, devocionais, fontes, decisoes, sinteses ou perguntas se eles nao vierem de uma fonte real do usuario.

A IA so pode criar notas, conceitos, entidades, projetos, fontes ou sinteses quando:

1. O usuario adicionar uma fonte real.
2. O usuario escrever uma nota real.
3. O usuario pedir explicitamente para criar aquele conteudo.
4. O conteudo ja existir no vault e precisar ser processado.

Se precisar demonstrar uma estrutura, usar placeholders genericos dentro de templates, nunca arquivos reais.

Exemplo correto:

- `90-system/templates/entity-template.md`

Exemplo incorreto:

- `03-wiki/entities/davi.md`, se o usuario nao adicionou uma fonte real sobre Davi.

## Estrutura principal

- `00-inbox/`: entrada livre e rapida para capturas ainda caoticas.
- `01-raw/`: fontes brutas e originais.
- `02-domains/`: grandes areas da vida humana.
- `03-wiki/`: conhecimento estruturado e conectado.
- `04-maps/`: mapas de navegacao e visao geral.
- `05-projects/`: projetos confirmados ou em avaliacao.
- `06-outputs/`: saidas finais geradas pela IA.
- `07-reviews/`: revisoes periodicas.
- `90-system/`: sistema interno, manuais, templates e regras.
- `99-archive/`: conteudo arquivado, antigo ou que precisa de revisao.

Nao deve existir `raw/` solto na raiz.

Nao deve existir `wiki/` solto na raiz.

## Fluxo profissional

O fluxo principal do sistema e:

Capturar -> Classificar -> Processar -> Conectar -> Sintetizar -> Revisar -> Reutilizar

1. Capturar: o usuario joga uma ideia em `00-inbox/` ou uma fonte em `01-raw/inbox/`.
2. Classificar: a IA identifica dominio principal, dominios secundarios, tipo de fonte, conceitos, entidades e projetos relacionados.
3. Processar: a IA cria uma nota limpa no local correto somente a partir de conteudo real.
4. Conectar: a IA cria links internos com conceitos, entidades, projetos, decisoes e fontes reais.
5. Sintetizar: a IA atualiza paginas de sintese somente quando houver conteudo real suficiente.
6. Revisar: a IA identifica padroes, lacunas, notas orfas e proximos passos.
7. Reutilizar: o usuario consulta o proprio conhecimento acumulado para estudar, decidir e construir.

## Regras de seguranca

1. Nao apagar conteudo real existente sem pedido explicito.
2. Nao sobrescrever arquivos existentes sem preservar ou mesclar o conteudo util.
3. Se uma pasta ja existir, manter a pasta e complementar a estrutura.
4. Fontes brutas em `01-raw/` sao fontes originais e nao devem ser reescritas.
5. Se houver duvida sobre classificacao, manter em inbox ou mover para `99-archive/review-needed/`.
6. Se uma nota tocar em mais de uma area, escolher uma area principal e criar links cruzados.
7. Se nao houver certeza se algo e real, nao apagar: mover para `99-archive/review-needed/` e registrar no relatorio.

## Fluxo de fontes brutas

### 1. Captura inicial

Toda fonte nova entra primeiro em:

- `01-raw/inbox/`

ou diretamente no inbox da categoria, se a categoria ja for clara:

- Artigo novo: `01-raw/articles/inbox/`
- Video novo: `01-raw/videos/inbox/`
- Aula nova: `01-raw/classes/inbox/`
- Fonte de trabalho: `01-raw/work/inbox/`
- Fonte biblica: `01-raw/bible/inbox/`
- Reuniao: `01-raw/meetings/inbox/`

### 2. Classificacao

A IA identifica o tipo da fonte e move para o inbox da categoria correta.

### 3. Processamento

Ao processar uma fonte, a IA deve:

1. Ler a fonte bruta.
2. Criar nota processada no dominio correto em `02-domains/`, se houver conteudo real.
3. Criar ou atualizar conceitos em `03-wiki/concepts/`, somente quando forem reais e vierem da fonte.
4. Criar ou atualizar entidades em `03-wiki/entities/`, somente quando forem reais e vierem da fonte.
5. Criar ou atualizar sinteses em `03-wiki/synthesis/`, somente quando houver conteudo real suficiente.
6. Criar links internos.
7. Atualizar `index.md` e `log.md`.
8. Registrar a fonte usada.
9. Mover a fonte bruta para `processed/` da propria categoria.

### 4. Arquivamento

Se uma fonte for duplicada, antiga ou nao for util agora, mover para `archive/` da categoria correspondente.

Nao usar `01-raw/processed/` global.

## Estrutura de 01-raw

Cada categoria de fonte deve ter:

- `inbox/`
- `processed/`
- `archive/`

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

## Regras de processamento de notas

Ao processar uma nova nota:

1. Ler o conteudo.
2. Identificar o tipo da nota.
3. Identificar o dominio principal.
4. Identificar dominios secundarios.
5. Identificar conceitos reais.
6. Identificar entidades reais.
7. Identificar projetos relacionados, sem criar projeto ativo automaticamente.
8. Criar ou atualizar nota processada no local correto.
9. Criar links internos com `[[wikilinks]]`.
10. Atualizar `index.md` da area.
11. Atualizar `log.md` da area.
12. Atualizar `03-wiki/` quando houver conceito ou entidade real relevante.
13. Atualizar `synthesis/` quando o tema for recorrente e houver base real suficiente.
14. Registrar duvidas em `questions/` somente quando surgirem de conteudo real.
15. Preservar a fonte original.

## Regras para classificacao

- Pensamento rapido: `00-inbox/`.
- Fonte original: `01-raw/`.
- Area da vida: `02-domains/`.
- Conceito reutilizavel real: `03-wiki/concepts/`.
- Pessoa, personagem, empresa, ferramenta, lugar ou projeto real: `03-wiki/entities/`.
- Visao geral: `04-maps/`.
- Projeto ainda nao confirmado: `05-projects/inbox/` ou `02-domains/05-projects-ideas/`.
- Projeto ativo confirmado: `05-projects/active/`.
- Saida final: `06-outputs/`.
- Revisao: `07-reviews/`.
- Conteudo antigo ou incerto: `99-archive/`.

## Regras para projetos

- Nao criar projeto automaticamente so porque ele apareceu em exemplo, prompt ou manual.
- Se o usuario mencionar um possivel projeto em uma nota, registrar primeiro em `05-projects/inbox/` ou `02-domains/05-projects-ideas/`.
- Criar projeto ativo em `05-projects/active/` somente quando o usuario pedir explicitamente ou confirmar que o projeto existe.

## Context Memories

Context Memories sao memorias recorrentes por assunto.

Antes de responder ou processar conteudo relacionado a um dominio, projeto ou assunto, o agente deve verificar se existem memorias contextuais relevantes.

O agente deve criar uma memoria contextual quando o usuario pedir explicitamente ou quando ele disser que algo deve ser lembrado recorrentemente.

Memorias devem ser salvas em:

`02-domains/[dominio]/memory/`

O agente nunca deve criar memoria ficticia.

## Regras de links

Use links internos no formato `[[nome-do-conceito]]`.

Sempre que possivel, conecte conteudos reais:

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

Nao criar a pagina linkada se ela ainda nao tiver conteudo real ou pedido explicito do usuario.

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
- `context-memory`

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

## Domain Pack

Cada dominio em `02-domains/` deve conter:

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

Antes de processar uma nota dentro de um dominio, leia o `_manual.md` daquele dominio.

A pasta `memory/` guarda memorias recorrentes daquele dominio. Sao lembretes persistentes que a IA deve considerar quando o assunto aparecer novamente.

Conteudo dentro do dominio so deve ser criado a partir de notas reais, fontes reais, conteudo ja existente ou pedido explicito do usuario.

## Regras para consultas

Ao responder uma pergunta:

1. Ler `index.md` primeiro.
2. Verificar se existem memorias contextuais relevantes em `02-domains/[dominio]/memory/`.
3. Ler paginas relevantes em `02-domains/`, `03-wiki/`, `04-maps/` e `05-projects/`.
4. Consultar fontes em `01-raw/` quando a resposta depender da origem.
5. Responder com citacoes para paginas do vault e caminhos de fontes quando disponiveis.
6. Se a resposta tiver valor duravel, registrar em uma pagina adequada somente com autorizacao ou base real clara.

## Quando tiver duvida

Se a IA nao souber onde colocar uma nota:

1. Nao inventar.
2. Colocar em `00-inbox/para-processar/` ou `01-raw/inbox/`, conforme o tipo.
3. Criar observacao no `log.md`.
4. Sugerir 2 ou 3 classificacoes provaveis quando isso ajudar.
