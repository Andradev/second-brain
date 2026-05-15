# AGENTS.md

## Proposito do Second Brain

Este vault e um Second Brain Universal com IA.

Ele existe para capturar, organizar, conectar e sintetizar o conhecimento pessoal do usuario ao longo da vida. A IA atua como bibliotecaria, analista de conhecimento, arquiteta de informacao, mentora de estudo e mantenedora de uma wiki viva.

## Principio central

Captura simples.

Organizacao depois.

LLM Wiki por baixo.

O usuario nao precisa entender a arquitetura inteira para usar o sistema. A interface humana deve ser pequena, clara e facil de lembrar.

## Interface humana simplificada

O usuario deve interagir principalmente com:

- `00-inbox/`
- `01-fontes/`
- `02-areas/`
- `03-projetos/`
- `04-revisoes/`
- `05-saidas/`

A parte tecnica fica em:

- `90-sistema/`

Coisas antigas, pausadas, descartadas ou incertas ficam em:

- `99-arquivo/`

## Regra de captura

Se veio da cabeca do usuario, vai para `00-inbox/`.

Se veio de fonte externa, documento, video, artigo, PDF, aula, print, transcricao ou material de referencia, vai para `01-fontes/inbox/`.

Se ja virou projeto candidato claro, vai para `03-projetos/inbox/`.

Depois disso, a IA organiza.

## Estrutura principal

- `START-HERE.md`: entrada visual e curta para o usuario.
- `README.md`: explicacao simples do sistema.
- `AGENTS.md`: regras operacionais para agentes de IA.
- `00-inbox/`: ideias soltas, duvidas, pensamentos e capturas rapidas.
- `01-fontes/`: fontes brutas externas preservadas.
- `02-areas/`: vida organizada em poucas areas humanas.
- `03-projetos/`: projetos candidatos, ativos, pausados e concluidos.
- `04-revisoes/`: revisoes semanais e mensais.
- `05-saidas/`: materiais finais.
- `90-sistema/`: nucleo tecnico, prompts, templates, regras e LLM Wiki.
- `99-arquivo/`: conteudo antigo, pausado, descartado ou que precisa de revisao.

Nao deve existir `01-raw/`, `02-domains/`, `03-wiki/`, `04-maps/`, `05-projects/`, `06-outputs/`, `07-reviews/`, `90-system/` ou `99-archive/` soltos na raiz.

## Nucleo LLM Wiki

O LLM Wiki continua existindo internamente em:

`90-sistema/llm-wiki/`

A IA deve usar esse nucleo para manter:

- fontes brutas preservadas
- fontes processadas
- notas organizadas
- conceitos
- entidades
- sinteses
- perguntas abertas
- comparacoes
- indices
- logs
- links internos
- atualizacao incremental

O usuario nao deve ser obrigado a navegar pelo nucleo tecnico para usar o vault.

## Relacao entre interface e LLM Wiki

- `01-fontes/` e a camada de fontes brutas.
- `02-areas/` e a camada de notas humanas organizadas por contexto de vida.
- `90-sistema/llm-wiki/wiki/` e a camada de conhecimento conectado.

Fluxo esperado:

1. O usuario captura em `00-inbox/` ou `01-fontes/inbox/`.
2. A IA classifica quando for solicitada.
3. A IA preserva a fonte original.
4. A IA cria notas organizadas em `02-areas/` somente com base real.
5. A IA atualiza conceitos, entidades, sinteses, perguntas e comparacoes em `90-sistema/llm-wiki/wiki/`.
6. A IA atualiza indices e logs relevantes.

## Regra contra conteudo simulado

A IA nunca deve criar conteudo ficticio, simulado ou baseado apenas em exemplos de documentacao.

Exemplos em manuais, prompts e templates servem apenas para orientar comportamento.

Nao criar arquivos sobre pessoas, personagens, projetos, conceitos, estudos, devocionais, fontes, decisoes, sinteses ou perguntas se eles nao vierem de:

1. Fonte real adicionada pelo usuario.
2. Nota real escrita pelo usuario.
3. Pedido explicito do usuario.
4. Conteudo real ja existente no vault.

Se precisar demonstrar uma estrutura, usar placeholders genericos dentro de templates, nunca arquivos reais.

## Fontes

Fonte externa nova entra em:

`01-fontes/inbox/`

Fonte ja usada pela IA vai para:

`01-fontes/processadas/`

Fonte antiga ou nao usada agora vai para:

`01-fontes/arquivadas/`

Fontes brutas sao originais e nao devem ser reescritas. Ao processar uma fonte, criar notas derivadas em outro lugar e preservar o arquivo original.

## Areas

As areas visiveis comecam simples:

- `02-areas/trabalho/`
- `02-areas/estudos/`
- `02-areas/fe-e-valores/`
- `02-areas/vida-pessoal/`
- `02-areas/ideias/`

Nao criar novas areas sem necessidade real. Se uma area crescer demais, criar proposta em `90-sistema/evolucao/proposals/` antes de mudar a estrutura.

## Projetos

Nao criar projeto ativo automaticamente.

Ideia quase pronta para virar projeto vai para `03-projetos/inbox/`.

Projeto ativo so entra em `03-projetos/ativos/` quando o usuario pedir explicitamente ou confirmar que o projeto existe.

Projetos pausados ficam em `03-projetos/pausados/`.

Projetos concluidos ficam em `03-projetos/concluidos/`.

## Revisoes

Revisoes periodicas ficam em `04-revisoes/`.

Comecar simples:

- `04-revisoes/semanais/`
- `04-revisoes/mensais/`

Uma revisao deve observar o que entrou, padroes recorrentes, fontes pendentes, tarefas, duvidas, projetos que precisam de atencao e temas que merecem virar wiki interna.

## Saidas

Materiais prontos ficam em `05-saidas/`.

Use esta pasta para documentos finais, prompts uteis, resumos, guias e relatorios.

Rascunhos e capturas soltas nao devem comecar aqui.

## Context memories

Memorias contextuais sao lembrancas recorrentes por dominio, contexto ou assunto.

A IA deve verificar memorias relacionadas antes de responder sobre um assunto, processar uma nota ou trabalhar em um projeto.

Memorias contextuais so devem ser criadas quando o usuario pedir explicitamente ou disser que algo deve ser lembrado de forma recorrente.

As regras e templates ficam em:

`90-sistema/memoria-contextual/`

Nao criar memorias ficticias.

## Evolucao do sistema

System Evolution e o modulo de evolucao controlada do Second Brain.

A IA pode observar padroes, assuntos recorrentes, areas que cresceram demais, templates faltantes, automacoes possiveis e oportunidades de melhoria.

Propostas ficam em:

`90-sistema/evolucao/proposals/`

A IA nao deve implementar mudancas estruturais medias ou grandes sem confirmacao humana.

Mudancas como criar nova area, alterar `AGENTS.md`, reorganizar muitos arquivos ou criar automacao exigem aprovacao explicita.

## Biblioteca de prompts

A biblioteca fica em:

`90-sistema/prompts/`

Esses prompts orientam tarefas operacionais. A IA pode consultar a biblioteca para escolher o prompt adequado, mas nao deve executar todos automaticamente.

Prompts que alteram conteudo real devem ser executados em branch separada, nunca diretamente na main.

## Templates

Templates ficam em:

`90-sistema/templates/`

Templates podem conter placeholders genericos. Eles nao contam como conteudo real.

## Regras de seguranca

1. Nao apagar conteudo real sem pedido explicito.
2. Nao sobrescrever arquivos existentes sem preservar ou mesclar o conteudo util.
3. Se uma pasta ja existir, manter a pasta e complementar a estrutura.
4. Se houver duvida sobre classificacao, manter em `00-inbox/para-processar/`, `01-fontes/inbox/` ou mover para `99-arquivo/revisar/`.
5. Se uma nota tocar em mais de uma area, escolher uma area principal e criar links cruzados.
6. Se nao houver certeza se algo e real, nao apagar.
7. Nao processar fontes sem pedido ou contexto claro.
8. Nao executar automacoes sem pedido explicito.
9. Nao fazer merge automatico.
10. Manter a main limpa quando o vault estiver sendo usado como template.

## Regras de processamento

Ao processar uma nota ou fonte real:

1. Ler o conteudo.
2. Identificar o tipo.
3. Identificar area principal.
4. Identificar areas secundarias.
5. Identificar conceitos reais.
6. Identificar entidades reais.
7. Identificar projetos relacionados sem criar projeto ativo automaticamente.
8. Criar ou atualizar nota processada no local correto.
9. Criar links internos com `[[wikilinks]]`.
10. Atualizar indices quando houver valor real.
11. Atualizar `90-sistema/llm-wiki/wiki/` quando houver conceito, entidade, pergunta, comparacao ou sintese relevante.
12. Registrar duvidas somente quando surgirem de conteudo real.
13. Preservar a fonte original.

## Regras de links

Use links internos no formato `[[nome-do-conceito]]`.

Sempre que possivel, conecte conteudos reais:

- nota com conceito
- conceito com entidade
- entidade com projeto
- projeto com decisao
- fonte com sintese
- diario com aprendizado
- estudo com projeto pratico
- devocional com personagem biblico
- trabalho com regra de negocio
- ideia com possivel projeto

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
- Evitar linguagem tecnica desnecessaria para o usuario.

## Frontmatter padrao

Notas processadas devem usar este frontmatter:

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
- `evolution-proposal`
- `evolution-analysis`

`status` pode ser:

- `inbox`
- `draft`
- `processing`
- `processed`
- `reviewed`
- `archived`
- `pending`
- `accepted`
- `rejected`
- `implemented`

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

Atualizacoes da LLM Wiki devem ser registradas em:

`90-sistema/llm-wiki/log.md`

Quando fizer sentido, use o formato:

```md
## YYYY-MM-DD

- Processado: [[arquivo-original]]
- Criado: [[nova-nota]]
- Atualizado: [[conceito]], [[entidade]], [[sintese]]
- Observacoes:
- Pendencias:
```

Nao criar relatorios historicos soltos na raiz.

## Ordem de consulta antes de responder

Quando receber uma tarefa, considerar:

1. `AGENTS.md`
2. `START-HERE.md` e `README.md`, se a duvida for sobre uso geral
3. regras em `90-sistema/regras/`
4. manuais ou templates relevantes em `90-sistema/`
5. memorias contextuais relacionadas
6. paginas relevantes em `02-areas/`
7. wiki interna em `90-sistema/llm-wiki/wiki/`
8. projetos relacionados em `03-projetos/`
9. fontes relacionadas em `01-fontes/`

## Regras para consultas

Ao responder uma pergunta baseada no vault:

1. Ler paginas relevantes em `02-areas/`, `90-sistema/llm-wiki/wiki/`, `03-projetos/` e `05-saidas/`.
2. Consultar fontes em `01-fontes/` quando a resposta depender da origem.
3. Responder com citacoes para paginas do vault e caminhos de fontes quando disponiveis.
4. Se a resposta tiver valor duravel, registrar em uma pagina adequada somente com autorizacao ou base real clara.

## Quando tiver duvida

Se a IA nao souber onde colocar algo:

1. Nao inventar.
2. Colocar pensamento solto em `00-inbox/para-processar/`.
3. Colocar fonte externa em `01-fontes/inbox/`.
4. Colocar conteudo incerto em `99-arquivo/revisar/`.
5. Sugerir duas ou tres classificacoes provaveis quando isso ajudar.
