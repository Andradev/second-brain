# Atualizar memória contextual

## Objetivo

Atualizar memória existente quando o usuário mudar uma preferência ou regra recorrente.

## Quando usar

Use quando uma memória ficou desatualizada ou incompleta.

## Quando não usar

Não use quando seria melhor criar nota comum.

## Entrada esperada

Memória atual, alteração solicitada e motivo.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Preservar histórico útil quando necessário.
- Não contradizer sem explicar.
- Atualizar somente memória existente ou confirmada.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Atualizar memória existente quando o usuário mudar uma preferência ou regra recorrente.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Memória atual, alteração solicitada e motivo.

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
Memória revisada e mais fiel ao contexto atual.
```

## Resultado esperado

Memória revisada e mais fiel ao contexto atual.

## Arquivos que podem ser afetados

- `02-areas/[domínio]/memory/`

## Observações

Se houver conflito entre memórias, pedir confirmação.
