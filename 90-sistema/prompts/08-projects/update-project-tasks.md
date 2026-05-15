# Atualizar tarefas do projeto

## Objetivo

Atualizar lista de tarefas de um projeto com ações reais.

## Quando usar

Use quando houver novas ações confirmadas ou extraídas de nota real.

## Quando não usar

Não use quando as ações forem meras possibilidades vagas.

## Entrada esperada

Projeto e ações com origem.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não inventar tarefas.
- Distinguir pendente, em andamento e concluído.
- Não apagar tarefa sem confirmação.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Atualizar lista de tarefas de um projeto com ações reais.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Projeto e ações com origem.

Tarefa:
1. Verifique o escopo solicitado.
2. Consulte regras, manuais e memórias contextuais relevantes quando aplicável.
3. Execute apenas a tarefa descrita neste prompt.
4. Preserve conteúdo real e registre dúvidas quando houver incerteza.
5. Ao final, informe o que foi criado, atualizado, movido ou deixado pendente.

Regras:
1. Não criar conteúdo simulado.
2. Não inventar informações.
3. Não apagar conteúdo real.
4. Respeitar a estrutura do Second Brain.
5. Registrar alterações quando necessário.
6. Se houver dúvida relevante, pedir confirmação ou mover para 99-arquivo/revisar.
7. Não fazer merge automático.

Resultado esperado:
Tarefas do projeto atualizadas.
```

## Resultado esperado

Tarefas do projeto atualizadas.

## Arquivos que podem ser afetados

- `03-projetos/ativos/[projeto]/`

## Observações

Tarefa deve ser acionável ou claramente exploratória.
