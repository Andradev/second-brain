# Rejeitar proposta de evolução

## Objetivo

Registrar rejeição ou arquivamento de proposta.

## Quando usar

Use quando o usuário rejeitar a proposta ou decidir adiar.

## Quando não usar

Não use quando a proposta precisa apenas de ajustes.

## Entrada esperada

Caminho da proposta e motivo.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não apagar proposta sem pedido.
- Registrar motivo.
- Preservar aprendizado.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Registrar rejeição ou arquivamento de proposta.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Caminho da proposta e motivo.

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
Proposta rejeitada ou arquivada com rastreabilidade.
```

## Resultado esperado

Proposta rejeitada ou arquivada com rastreabilidade.

## Arquivos que podem ser afetados

- `90-system/evolution/proposals/`

## Observações

Rejeições ajudam o sistema a não repetir sugestões ruins.
