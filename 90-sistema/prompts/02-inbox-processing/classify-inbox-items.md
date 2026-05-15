# Classificar itens de inbox

## Objetivo

Classificar itens de inbox sem necessariamente processar o conteúdo completo.

## Quando usar

Use quando houver muitos itens e o primeiro passo for triagem.

## Quando não usar

Não use quando o usuário pedir processamento completo de uma fonte específica.

## Entrada esperada

Pasta de inbox ou lista de itens a classificar.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não reescrever conteúdo original.
- Não excluir itens.
- Marcar incertezas.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Classificar itens de inbox sem necessariamente processar o conteúdo completo.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Pasta de inbox ou lista de itens a classificar.

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
Lista de itens com destino sugerido e motivo.
```

## Resultado esperado

Lista de itens com destino sugerido e motivo.

## Arquivos que podem ser afetados

- `00-inbox/`
- `02-areas/*/inbox/`
- `01-fontes/inbox/`
- `99-arquivo/revisar/`

## Observações

Bom para reduzir ambiguidade antes de operações maiores.
