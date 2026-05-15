# Mover fonte para processadas

## Objetivo

Mover uma fonte bruta para `01-fontes/processadas/` depois de processamento real.

## Quando usar

Use quando a fonte ja foi lida, registrada e usada para criar ou atualizar conhecimento real.

## Quando nao usar

Nao use quando a fonte ainda nao foi processada ou quando restarem duvidas importantes.

## Entrada esperada

Caminho da fonte e referencia da nota, conceito, entidade ou sintese criada ou atualizada.

## Regras importantes

- Nao criar conteudo simulado.
- Nao inventar informacoes ausentes.
- Nao apagar conteudo real.
- Confirmar que a nota processada ou atualizacao existe.
- Usar `01-fontes/processadas/` como destino unico.
- Preservar a fonte original.

## Prompt copiavel

```txt
Voce e um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Mover uma fonte de `01-fontes/inbox/` para `01-fontes/processadas/` apos processamento real.

Tarefa:
1. Verifique se a fonte foi realmente processada.
2. Confirme quais notas, conceitos, entidades ou sinteses foram criados ou atualizados.
3. Preserve a fonte original.
4. Mova a fonte para `01-fontes/processadas/`.
5. Informe o que foi movido e qual conhecimento foi gerado.
```

## Resultado esperado

Fonte preservada em `01-fontes/processadas/` com rastreabilidade clara.
