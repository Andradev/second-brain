# Identificar conceitos do domínio

## Objetivo

Extrair conceitos reais recorrentes ou reutilizáveis de notas de um domínio.

## Quando usar

Use quando há notas reais suficientes para identificar conceitos.

## Quando não usar

Não use quando há apenas uma menção vaga ou exemplo de prompt.

## Entrada esperada

Notas ou fontes reais do domínio.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não criar conceito vazio.
- Diferenciar termo casual de conceito reutilizável.
- Atualizar wiki apenas quando houver base suficiente.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Extrair conceitos reais recorrentes ou reutilizáveis de notas de um domínio.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Notas ou fontes reais do domínio.

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
Lista de conceitos candidatos com origem e recomendação.
```

## Resultado esperado

Lista de conceitos candidatos com origem e recomendação.

## Arquivos que podem ser afetados

- `02-domains/[domínio]/concepts/`
- `03-wiki/concepts/`

## Observações

Pode sugerir sem criar se a base ainda for fraca.
