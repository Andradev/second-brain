# Preservar trabalho atual

## Objetivo

Proteger alterações existentes antes de iniciar nova tarefa.

## Quando usar

Use quando há git status sujo ou mudanças do usuário.

## Quando não usar

Não use quando a árvore está limpa e a tarefa é simples.

## Entrada esperada

Status atual e nova tarefa desejada.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não sobrescrever mudanças.
- Identificar arquivos alterados.
- Pedir orientação se houver conflito.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Proteger alterações existentes antes de iniciar nova tarefa.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Status atual e nova tarefa desejada.

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
6. Se houver dúvida relevante, pedir confirmação ou mover para review-needed.
7. Não fazer merge automático.

Resultado esperado:
Trabalho atual preservado antes de prosseguir.
```

## Resultado esperado

Trabalho atual preservado antes de prosseguir.

## Arquivos que podem ser afetados

- `Git`
- Arquivos alterados existentes

## Observações

Preservar é diferente de commitar; escolha depende do contexto.
