# Gerar resumo de mudança

## Objetivo

Gerar resumo final de alterações feitas pelo Codex.

## Quando usar

Use após concluir uma tarefa real de edição.

## Quando não usar

Não use quando nada foi alterado.

## Entrada esperada

Git status/diff e objetivo original.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Relatar apenas alterações reais.
- Incluir validações feitas.
- Apontar problemas.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Gerar resumo final de alterações feitas pelo Codex.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Git status/diff e objetivo original.

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
Resumo final com arquivos principais e sugestão de commit.
```

## Resultado esperado

Resumo final com arquivos principais e sugestão de commit.

## Arquivos que podem ser afetados

- `Git`
- Arquivos alterados

## Observações

Resumo não deve fingir testes não executados.
