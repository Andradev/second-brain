# Criar ajuste estrutural a partir de proposta

## Objetivo

Criar área, subpasta ou ajuste estrutural somente após aprovação.

## Quando usar

Use quando uma proposta aprovada pede uma mudança estrutural.

## Quando não usar

Não use quando só há um tema recorrente sem decisão humana.

## Entrada esperada

Proposta aprovada, nome da mudança e área relacionada.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Confirmar aprovação.
- Criar estrutura mínima necessária.
- Não migrar conteúdo sem escopo.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Criar área, subpasta ou ajuste estrutural somente após aprovação.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Proposta aprovada, nome da mudança e área relacionada.

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
Ajuste estrutural criado conforme proposta.
```

## Resultado esperado

Ajuste estrutural criado conforme proposta.

## Arquivos que podem ser afetados

- `02-areas/`
- `90-sistema/evolucao/`

## Observações

Nova estrutura não deve virar depósito vazio sem propósito.
