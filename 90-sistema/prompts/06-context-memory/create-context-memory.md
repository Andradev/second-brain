# Criar memória contextual

## Objetivo

Criar uma memória persistente de contexto quando o usuário pedir explicitamente.

## Quando usar

Use quando o usuário disser para lembrar algo de forma recorrente.

## Quando não usar

Não use quando a informação for apenas uma nota comum ou hipótese.

## Entrada esperada

Domínio, contexto, conteúdo da memória e gatilho de uso.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Confirmar que é memória recorrente.
- Não criar memória fictícia.
- Escrever de forma curta e operacional.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Criar uma memória persistente de contexto quando o usuário pedir explicitamente.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Domínio, contexto, conteúdo da memória e gatilho de uso.

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
Memória criada no domínio correto.
```

## Resultado esperado

Memória criada no domínio correto.

## Arquivos que podem ser afetados

- `02-areas/[domínio]/memory/`

## Observações

Memória deve orientar respostas futuras, não duplicar notas.
