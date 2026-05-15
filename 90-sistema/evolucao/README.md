# Evolução do sistema

## O que é este módulo

System Evolution é o módulo responsável por observar como o Second Brain está crescendo.

Ele ajuda a identificar padrões de uso, assuntos recorrentes, temas repetidos, novas áreas de interesse e possíveis melhorias estruturais.

## Para que serve

Este módulo serve para criar propostas de evolução antes de alterar a arquitetura do vault.

A IA pode observar, analisar e propor melhorias como:

- Criar nova área, se houver necessidade real.
- Criar nova pasta especializada dentro da estrutura atual.
- Criar nova seção interna da LLM Wiki.
- Criar novo template.
- Criar nova regra para `AGENTS.md`.
- Criar nova automação.
- Criar nova memória contextual.
- Reorganizar uma área que ficou grande demais.

## Regra central

A autoevolução deve ser controlada.

A IA pode observar, analisar e propor.

A IA não deve aplicar mudanças estruturais médias ou grandes sem confirmação explícita do usuário.

## Onde ficam as propostas

Propostas de evolução ficam em:

```md
90-sistema/evolucao/proposals/
```

Estados possíveis:

- `pending/`: propostas aguardando revisão.
- `accepted/`: propostas aprovadas.
- `rejected/`: propostas rejeitadas.
- `implemented/`: propostas já implementadas.

## Arquivos deste módulo

- `evolution-rules.md`: regras de evolução controlada.
- `proposal-template.md`: template geral de proposta.
- `domain-evolution-template.md`: template para análise de evolução de área.
- `recurring-topic-analysis-template.md`: template de análise de temas recorrentes.
- `proposals/`: propostas separadas por status.
- `logs/`: registros de análises de evolução.

## O que não fazer

Não criar nova área global automaticamente.

Não mover grandes quantidades de arquivos automaticamente.

Não alterar `AGENTS.md` sem explicar claramente a mudança.

Não criar conteúdo simulado.
