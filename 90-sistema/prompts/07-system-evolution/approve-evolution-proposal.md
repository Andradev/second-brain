# Aprovar proposta de evolução

## Objetivo

Registrar aprovação humana de uma proposta existente.

## Quando usar

Use quando o usuário aprovar explicitamente uma proposta.

## Quando não usar

Não use quando a proposta ainda não foi revisada.

## Entrada esperada

Caminho da proposta e confirmação do usuário.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Verificar status atual.
- Não implementar se aprovação for ambígua.
- Registrar aprovação.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Registrar aprovação humana de uma proposta existente.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Caminho da proposta e confirmação do usuário.

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
Proposta marcada como aceita ou pronta para implementação.
```

## Resultado esperado

Proposta marcada como aceita ou pronta para implementação.

## Arquivos que podem ser afetados

- `90-sistema/evolution/proposals/`

## Observações

Aprovar não significa executar tudo sem plano.
