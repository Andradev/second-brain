# Criar página de entidade

## Objetivo

Criar página para pessoa, ferramenta, empresa, lugar ou projeto real.

## Quando usar

Use quando entidade real aparece em conteúdo do vault.

## Quando não usar

Não use quando é personagem, pessoa ou ferramenta citada só como exemplo.

## Entrada esperada

Nome da entidade, tipo e origem real.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não inventar biografia.
- Registrar apenas dados conhecidos.
- Não criar projeto ativo por implicação.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Criar página para pessoa, ferramenta, empresa, lugar ou projeto real.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Nome da entidade, tipo e origem real.

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
Página de entidade rastreável e enxuta.
```

## Resultado esperado

Página de entidade rastreável e enxuta.

## Arquivos que podem ser afetados

- `90-sistema/llm-wiki/wiki/entities/`

## Observações

Para entidades sensíveis, manter descrição mínima.
