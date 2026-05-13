# Processar imports em branch

## Objetivo

Trabalhar imports ou lotes de conteúdo em branch isolada.

## Quando usar

Use quando há muitos arquivos novos a classificar/processar.

## Quando não usar

Não use quando o processamento é de um único arquivo simples.

## Entrada esperada

Origem dos imports e objetivo do lote.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Criar branch específica.
- Preservar originais.
- Processar em etapas verificáveis.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Trabalhar imports ou lotes de conteúdo em branch isolada.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Origem dos imports e objetivo do lote.

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
Imports processados sem afetar main.
```

## Resultado esperado

Imports processados sem afetar main.

## Arquivos que podem ser afetados

- `00-inbox/`
- `01-raw/`
- `02-domains/`
- `Git`

## Observações

Lotes grandes devem ter checkpoints.
