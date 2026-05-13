# Encontrar notas órfãs

## Objetivo

Encontrar notas com poucos ou nenhum link interno.

## Quando usar

Use quando o usuário quiser melhorar conexão do conhecimento.

## Quando não usar

Não use quando a nota ainda está em inbox e não foi processada.

## Entrada esperada

Escopo de busca.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não criar links artificiais.
- Sugerir conexões apenas com base real.
- Não alterar automaticamente se incerto.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Encontrar notas com poucos ou nenhum link interno.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Escopo de busca.

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
Lista de notas órfãs e conexões candidatas.
```

## Resultado esperado

Lista de notas órfãs e conexões candidatas.

## Arquivos que podem ser afetados

- `02-domains/`
- `03-wiki/`

## Observações

Nem toda nota órfã é problema.
