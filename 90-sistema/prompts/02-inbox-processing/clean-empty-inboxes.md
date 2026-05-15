# Limpar inboxes vazios

## Objetivo

Remover ou padronizar marcadores vazios em inboxes sem apagar conteúdo real.

## Quando usar

Use quando inboxes estão vazios mas têm arquivos placeholders ou ruído estrutural.

## Quando não usar

Não use quando houver qualquer arquivo com conteúdo real não revisado.

## Entrada esperada

Lista de inboxes a verificar.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Verificar se os arquivos estão realmente vazios.
- Não apagar conteúdo real.
- Pedir confirmação antes de remover arquivos duvidosos.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Remover ou padronizar marcadores vazios em inboxes sem apagar conteúdo real.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Lista de inboxes a verificar.

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
Inboxes ficam limpos mantendo estrutura e conteúdo real preservado.
```

## Resultado esperado

Inboxes ficam limpos mantendo estrutura e conteúdo real preservado.

## Arquivos que podem ser afetados

- `00-inbox/`
- `01-fontes/*/inbox/`
- `02-areas/*/inbox/`

## Observações

Se houver dúvida, não remova: mova para revisão ou peça confirmação.
