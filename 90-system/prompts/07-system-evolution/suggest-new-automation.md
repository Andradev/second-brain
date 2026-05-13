# Sugerir nova automação

## Objetivo

Sugerir automação a partir de fricção recorrente no sistema.

## Quando usar

Use quando uma tarefa repetitiva aparece com frequência.

## Quando não usar

Não use quando é uma ação única ou incerta.

## Entrada esperada

Descrição da rotina repetitiva e evidências.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Sugerir antes de implementar.
- Definir gatilho, escopo e risco.
- Aguardar confirmação.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Sugerir automação a partir de fricção recorrente no sistema.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Descrição da rotina repetitiva e evidências.

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
Sugestão de automação documentada.
```

## Resultado esperado

Sugestão de automação documentada.

## Arquivos que podem ser afetados

- `90-system/evolution/proposals/pending/`
- `90-system/automations/`

## Observações

Automação deve reduzir trabalho sem criar comportamento perigoso.
