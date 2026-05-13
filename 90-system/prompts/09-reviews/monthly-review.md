# Revisão mensal

## Objetivo

Criar revisão mensal com padrões mais amplos e decisões relevantes.

## Quando usar

Use no fechamento do mês.

## Quando não usar

Não use quando há apenas uma nota isolada.

## Entrada esperada

Mês, domínios prioritários e escopo.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Analisar tendências reais.
- Não transformar sugestão em decisão.
- Separar manutenção de conteúdo.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Criar revisão mensal com padrões mais amplos e decisões relevantes.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Mês, domínios prioritários e escopo.

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
Revisão mensal em `07-reviews/monthly/`.
```

## Resultado esperado

Revisão mensal em `07-reviews/monthly/`.

## Arquivos que podem ser afetados

- `07-reviews/monthly/`

## Observações

Útil para detectar temas recorrentes.
