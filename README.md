# Second Brain Universal com IA

Este sistema serve para capturar ideias, preservar fontes, organizar areas da vida, manter projetos, gerar revisoes e permitir que a IA construa uma wiki interna de conhecimento.

## Como usar

1. Ideias soltas vao para `00-inbox/`.
2. Fontes externas vao para `01-fontes/inbox/`.
3. Conteudos organizados ficam em `02-areas/`.
4. Projetos ficam em `03-projetos/`.
5. Revisoes ficam em `04-revisoes/`.
6. Materiais finais ficam em `05-saidas/`.
7. A parte tecnica fica em `90-sistema/`.

## A regra mais simples

Se veio da sua cabeca, coloque em `00-inbox/`.

Se veio de fora, coloque em `01-fontes/inbox/`.

Depois a IA organiza.

## O que acontece por baixo

A IA usa uma arquitetura LLM Wiki interna para conectar conhecimento.

Essa wiki interna fica em:

`90-sistema/llm-wiki/`

Voce nao precisa mexer nela no dia a dia.

## Pastas principais

- `00-inbox/`: coisas soltas.
- `01-fontes/`: fontes externas preservadas.
- `02-areas/`: vida organizada por contexto.
- `03-projetos/`: projetos candidatos, ativos, pausados e concluidos.
- `04-revisoes/`: revisoes semanais e mensais.
- `05-saidas/`: materiais prontos.
- `90-sistema/`: regras, templates, prompts e nucleo LLM Wiki.
- `99-arquivo/`: coisas antigas, pausadas, descartadas ou incertas.

## Regra de ouro

Nao tente organizar tudo perfeitamente na hora.

Capture primeiro.

A IA organiza depois.
