# Criar página de pergunta

## Objetivo

Criar página para pergunta persistente conectada ao conhecimento do vault.

## Quando usar

Use quando a pergunta é recorrente ou importante.

## Quando não usar

Não use quando é uma dúvida pequena que cabe na nota de origem.

## Entrada esperada

Pergunta, origem e contexto.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não criar perguntas artificiais.
- Linkar notas relacionadas.
- Registrar estado atual da resposta.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Criar página para pergunta persistente conectada ao conhecimento do vault.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Pergunta, origem e contexto.

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
Pergunta navegável com contexto e próximos passos.
```

## Resultado esperado

Pergunta navegável com contexto e próximos passos.

## Arquivos que podem ser afetados

- `90-sistema/llm-wiki/wiki/questions/`

## Observações

Perguntas abertas devem permanecer honestamente abertas.
