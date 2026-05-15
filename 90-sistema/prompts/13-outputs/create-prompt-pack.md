# Criar pacote de prompts

## Objetivo

Criar um pack de prompts reutilizáveis para fluxo específico.

## Quando usar

Use quando vários prompts precisam ser usados em sequência documentada.

## Quando não usar

Não use quando um único prompt simples resolve.

## Entrada esperada

Nome do fluxo, prompts participantes e ordem.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não executar prompts do pack.
- Documentar sequência e critérios de parada.
- Usar exemplos conceituais.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Criar um pack de prompts reutilizáveis para fluxo específico.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Nome do fluxo, prompts participantes e ordem.

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
Pack criado em `90-sistema/prompts/packs/`.
```

## Resultado esperado

Pack criado em `90-sistema/prompts/packs/`.

## Arquivos que podem ser afetados

- `90-sistema/prompts/packs/`

## Observações

Pack é mapa de uso, não automação.
