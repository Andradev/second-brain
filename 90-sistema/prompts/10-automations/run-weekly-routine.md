# Rodar rotina semanal

## Objetivo

Executar rotina semanal documentada em branch segura.

## Quando usar

Use quando o usuário pedir rotina semanal.

## Quando não usar

Não use quando há dúvidas sobre escopo ou risco alto.

## Entrada esperada

Semana e áreas incluídas.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Criar/verificar branch.
- Não fazer merge automático.
- Separar revisão de processamento.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Executar rotina semanal documentada em branch segura.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Semana e áreas incluídas.

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
Rotina semanal concluída com pendências claras.
```

## Resultado esperado

Rotina semanal concluída com pendências claras.

## Arquivos que podem ser afetados

- `04-revisoes/weekly/`
- `01-fontes/`
- `02-areas/`

## Observações

Rotinas maiores podem exigir confirmação etapa a etapa.
