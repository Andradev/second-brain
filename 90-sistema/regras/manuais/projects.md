# Manual: Projetos

## Proposito

`03-projetos/` guarda projetos reais confirmados pelo usuario e ideias que talvez virem projetos.

## Estrutura

- `inbox/`: ideias que talvez virem projetos, mas ainda nao foram formalizadas.
- `ativos/`: projetos ativos criados ou confirmados pelo usuario.
- `pausados/`: projetos pausados.
- `concluidos/`: projetos concluidos.

## Regras

- Nao criar projeto automaticamente so porque ele foi citado em um exemplo.
- Nao criar projeto ativo sem pedido explicito ou confirmacao do usuario.
- Se uma nota mencionar um possivel projeto, registrar primeiro em `03-projetos/inbox/` ou em `02-areas/ideias/`.
- Se houver conteudo real suficiente mas nenhuma confirmacao, sugerir a criacao do projeto em vez de criar automaticamente.

## Estrutura recomendada para projeto ativo

Quando o usuario pedir para criar um projeto ativo, usar:

- `_manual.md`
- `index.md`
- `contexto.md`
- `tarefas.md`
- `decisoes.md`
- `notas/`
- `fontes/`
- `saidas/`

## Tarefas

Quando houver prioridade, usar:

```md
- Titulo da tarefa
  Descricao da tarefa
  #priority:P0
```

Prioridades validas: P0, P1, P2 e P3.
