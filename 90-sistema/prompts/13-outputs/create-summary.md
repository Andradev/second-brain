# Criar resumo

## Objetivo

Gerar resumo final de uma fonte, nota ou conjunto real.

## Quando usar

Use quando o usuário pedir síntese curta de material existente.

## Quando não usar

Não use quando a tarefa é criar página wiki permanente.

## Entrada esperada

Material a resumir e tamanho desejado.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não extrapolar além do material.
- Manter fidelidade.
- Indicar lacunas.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Gerar resumo final de uma fonte, nota ou conjunto real.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Material a resumir e tamanho desejado.

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
Resumo salvo ou entregue conforme pedido.
```

## Resultado esperado

Resumo salvo ou entregue conforme pedido.

## Arquivos que podem ser afetados

- `05-saidas/summaries/`

## Observações

Resumo final pode ser output ou permanecer no chat, conforme pedido.
