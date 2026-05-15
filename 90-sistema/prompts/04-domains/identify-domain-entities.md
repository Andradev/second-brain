# Identificar entidades do domínio

## Objetivo

Identificar pessoas, ferramentas, empresas, lugares ou projetos reais mencionados em um domínio.

## Quando usar

Use quando uma nota real contém entidades importantes.

## Quando não usar

Não use quando a entidade só aparece em exemplo conceitual.

## Entrada esperada

Notas ou fontes reais do domínio.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não criar entidade sem base real.
- Preservar contexto de origem.
- Não criar projeto ativo automaticamente.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Identificar pessoas, ferramentas, empresas, lugares ou projetos reais mencionados em um domínio.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Notas ou fontes reais do domínio.

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
Entidades candidatas ou páginas atualizadas com fonte.
```

## Resultado esperado

Entidades candidatas ou páginas atualizadas com fonte.

## Arquivos que podem ser afetados

- `02-areas/[domínio]/entities/`
- `90-sistema/llm-wiki/wiki/entities/`

## Observações

Se a entidade for sensível, manter mínimo necessário.
