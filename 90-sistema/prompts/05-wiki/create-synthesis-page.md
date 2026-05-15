# Criar página de síntese

## Objetivo

Criar síntese wiki a partir de múltiplas notas reais conectadas.

## Quando usar

Use quando há recorrência e material suficiente.

## Quando não usar

Não use quando há apenas uma nota ou fonte isolada.

## Entrada esperada

Tema da síntese e links das notas de base.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não preencher lacunas com invenção.
- Citar páginas de origem.
- Separar conclusões de perguntas.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Criar síntese wiki a partir de múltiplas notas reais conectadas.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Tema da síntese e links das notas de base.

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
Síntese conectada em `90-sistema/llm-wiki/wiki/synthesis/`.
```

## Resultado esperado

Síntese conectada em `90-sistema/llm-wiki/wiki/synthesis/`.

## Arquivos que podem ser afetados

- `90-sistema/llm-wiki/wiki/synthesis/`

## Observações

Síntese é resultado de acúmulo, não ponto de partida fictício.
