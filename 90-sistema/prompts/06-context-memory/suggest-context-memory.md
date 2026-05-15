# Sugerir memória contextual

## Objetivo

Sugerir que algo vire memória quando houver recorrência clara.

## Quando usar

Use quando um padrão aparece repetidamente em notas reais ou instruções do usuário.

## Quando não usar

Não use quando há só uma ocorrência isolada.

## Entrada esperada

Evidências de recorrência e domínio provável.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Sugerir, não criar automaticamente.
- Explicar benefício.
- Aguardar confirmação para criar.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Sugerir que algo vire memória quando houver recorrência clara.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Evidências de recorrência e domínio provável.

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
Sugestão de memória com texto proposto e motivo.
```

## Resultado esperado

Sugestão de memória com texto proposto e motivo.

## Arquivos que podem ser afetados

- Nenhum arquivo deve ser alterado sem confirmação

## Observações

Esse prompt é consultivo.
