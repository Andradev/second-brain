# Criar síntese de área

## Objetivo

Criar ou atualizar síntese de área quando houver conteúdo real suficiente.

## Quando usar

Use quando o tema é recorrente e há base real.

## Quando não usar

Não use quando há apenas uma nota isolada ou especulação.

## Entrada esperada

Conjunto de notas/fontes reais e tema da síntese.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não sintetizar além da base.
- Citar notas de origem.
- Marcar lacunas.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Criar ou atualizar síntese de área quando houver conteúdo real suficiente.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Conjunto de notas/fontes reais e tema da síntese.

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
Síntese útil conectando padrões reais da área.
```

## Resultado esperado

Síntese útil conectando padrões reais da área.

## Arquivos que podem ser afetados

- `90-sistema/llm-wiki/wiki/synthesis/`
- `90-sistema/llm-wiki/wiki/synthesis/`

## Observações

Síntese deve nascer de recorrência, não de vontade de preencher pasta.
