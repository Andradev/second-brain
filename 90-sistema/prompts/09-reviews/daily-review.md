# Revisão diária

## Objetivo

Gerar revisão diária a partir de capturas, notas e ações reais do dia.

## Quando usar

Use no fechamento de um dia de uso do vault.

## Quando não usar

Não use quando não houver conteúdo do período ou o usuário pediu só consulta.

## Entrada esperada

Data ou intervalo do dia e escopo.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não inventar eventos.
- Separar concluído, pendente e aprendizados.
- Não executar reorganizações grandes.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Gerar revisão diária a partir de capturas, notas e ações reais do dia.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Data ou intervalo do dia e escopo.

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
Revisão diária leve registrada em `00-inbox/para-processar/` ou considerada na próxima revisão semanal.
```

## Resultado esperado

Revisão diária leve registrada em `00-inbox/para-processar/` ou considerada na próxima revisão semanal.

## Arquivos que podem ser afetados

- `00-inbox/para-processar/`
- `04-revisoes/semanais/`

## Observações

Boa revisão diária é curta e acionável.
