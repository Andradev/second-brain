# Rodar manutenção mensal

## Objetivo

Executar manutenção mensal segura do vault.

## Quando usar

Use quando o usuário pedir manutenção mensal.

## Quando não usar

Não use quando existem alterações não revisadas que tornam o escopo perigoso.

## Entrada esperada

Mês, escopo e tarefas de manutenção permitidas.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Verificar git status.
- Não apagar conteúdo real.
- Pedir confirmação para limpezas duvidosas.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Executar manutenção mensal segura do vault.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Mês, escopo e tarefas de manutenção permitidas.

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
Manutenção mensal executada ou parcialmente planejada.
```

## Resultado esperado

Manutenção mensal executada ou parcialmente planejada.

## Arquivos que podem ser afetados

- `07-reviews/monthly/`
- `90-system/`
- `03-wiki/`

## Observações

Manutenção não deve reestruturar o vault inteiro sem proposta.
