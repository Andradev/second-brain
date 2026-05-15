# Registrar decisão de domínio

## Objetivo

Registrar uma decisão real relacionada a um domínio.

## Quando usar

Use quando o usuário tomou ou confirmou uma decisão.

## Quando não usar

Não use quando há apenas hipótese ou opção em aberto.

## Entrada esperada

Decisão, contexto, data e origem.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não transformar sugestão em decisão.
- Registrar motivos e consequências conhecidas.
- Linkar fontes reais.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Registrar uma decisão real relacionada a um domínio.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Decisão, contexto, data e origem.

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
Decisão registrada de forma rastreável.
```

## Resultado esperado

Decisão registrada de forma rastreável.

## Arquivos que podem ser afetados

- `02-areas/[domínio]/decisions/`
- `02-areas/[domínio]/log.md`

## Observações

Decisões devem ser explícitas.
