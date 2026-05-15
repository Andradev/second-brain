# Criar página de comparação

## Objetivo

Comparar conceitos, ferramentas, decisões ou abordagens com base real.

## Quando usar

Use quando há dois ou mais itens reais já presentes no vault.

## Quando não usar

Não use quando os itens são hipotéticos e sem fonte.

## Entrada esperada

Itens a comparar e páginas/fontes de origem.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Comparar apenas atributos existentes.
- Marcar desconhecidos como desconhecidos.
- Não forçar vencedor.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Comparar conceitos, ferramentas, decisões ou abordagens com base real.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Itens a comparar e páginas/fontes de origem.

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
Comparação útil, honesta e ligada às fontes.
```

## Resultado esperado

Comparação útil, honesta e ligada às fontes.

## Arquivos que podem ser afetados

- `90-sistema/llm-wiki/wiki/comparisons/`

## Observações

Comparações podem apoiar decisão, mas não substituem confirmação humana.
