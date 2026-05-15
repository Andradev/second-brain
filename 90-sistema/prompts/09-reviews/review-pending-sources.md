# Revisar fontes pendentes

## Objetivo

Revisar fontes ainda em inbox ou pendentes de processamento.

## Quando usar

Use quando `01-fontes/` acumular materiais não processados.

## Quando não usar

Não use quando o usuário pediu para processar uma fonte específica agora.

## Entrada esperada

Categorias de raw a revisar.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não processar automaticamente se o escopo for só revisão.
- Classificar prioridade.
- Não apagar fonte.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Revisar fontes ainda em inbox ou pendentes de processamento.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Categorias de raw a revisar.

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
Lista de fontes pendentes por prioridade e destino sugerido.
```

## Resultado esperado

Lista de fontes pendentes por prioridade e destino sugerido.

## Arquivos que podem ser afetados

- `01-fontes/*/inbox/`
- `04-revisoes/`

## Observações

Revisão ajuda escolher o próximo processamento.
