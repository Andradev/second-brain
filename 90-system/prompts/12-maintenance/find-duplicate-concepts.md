# Encontrar conceitos duplicados

## Objetivo

Detectar conceitos possivelmente duplicados no vault.

## Quando usar

Use quando conceitos parecem redundantes.

## Quando não usar

Não use quando é só diferença legítima de contexto.

## Entrada esperada

Escopo na wiki ou domínios.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não mesclar sem confirmação.
- Comparar origem e significado.
- Preservar conteúdo.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Detectar conceitos possivelmente duplicados no vault.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Escopo na wiki ou domínios.

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
Lista de duplicidades candidatas.
```

## Resultado esperado

Lista de duplicidades candidatas.

## Arquivos que podem ser afetados

- `03-wiki/concepts/`
- `02-domains/*/concepts/`

## Observações

Duplicidade precisa de revisão humana quando impacta links.
