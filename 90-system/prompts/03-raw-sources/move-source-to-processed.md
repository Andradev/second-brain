# Mover fonte para processed

## Objetivo

Mover uma fonte bruta para `processed/` da própria categoria após processamento real.

## Quando usar

Use quando uma fonte já foi processada e registrada.

## Quando não usar

Não use quando a fonte ainda não foi lida ou está pendente.

## Entrada esperada

Caminho da fonte e referência da nota processada criada.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Confirmar que a nota processada existe.
- Não usar `01-raw/processed/` global.
- Não apagar a fonte original.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Mover uma fonte bruta para `processed/` da própria categoria após processamento real.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Caminho da fonte e referência da nota processada criada.

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
Fonte movida para o processed correto com rastreabilidade mantida.
```

## Resultado esperado

Fonte movida para o processed correto com rastreabilidade mantida.

## Arquivos que podem ser afetados

- `01-raw/[categoria]/inbox/`
- `01-raw/[categoria]/processed/`

## Observações

Se houver dúvida, mantenha no inbox com observação.
