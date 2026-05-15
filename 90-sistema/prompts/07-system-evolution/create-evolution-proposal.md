# Criar proposta de evolução

## Objetivo

Criar uma proposta formal para mudança no sistema.

## Quando usar

Use quando uma melhoria estrutural tem evidências e escopo claro.

## Quando não usar

Não use quando a mudança pode ser feita como ajuste pequeno já autorizado.

## Entrada esperada

Problema, evidências, impacto e alternativa sugerida.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Criar proposta em pending.
- Não implementar automaticamente.
- Explicar riscos e rollback.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Criar uma proposta formal para mudança no sistema.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Problema, evidências, impacto e alternativa sugerida.

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
Proposta pendente documentada para revisão humana.
```

## Resultado esperado

Proposta pendente documentada para revisão humana.

## Arquivos que podem ser afetados

- `90-sistema/evolution/proposals/pending/`

## Observações

Propostas devem ser específicas.
