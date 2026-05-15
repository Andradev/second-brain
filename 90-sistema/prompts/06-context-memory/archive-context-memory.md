# Arquivar memória contextual

## Objetivo

Arquivar memória que não deve mais orientar respostas futuras.

## Quando usar

Use quando o usuário disser que uma memória não vale mais.

## Quando não usar

Não use quando a memória apenas precisa de ajuste.

## Entrada esperada

Memória a arquivar e motivo.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não apagar diretamente sem pedido explícito.
- Mover para arquivo quando aplicável.
- Registrar motivo.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Arquivar memória que não deve mais orientar respostas futuras.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Memória a arquivar e motivo.

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
Memória removida do fluxo ativo sem perda de rastreabilidade.
```

## Resultado esperado

Memória removida do fluxo ativo sem perda de rastreabilidade.

## Arquivos que podem ser afetados

- `02-areas/[domínio]/memory/`
- `99-arquivo/`

## Observações

Arquivar muda comportamento futuro do agente.
