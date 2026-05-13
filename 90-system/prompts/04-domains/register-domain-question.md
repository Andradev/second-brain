# Registrar pergunta de domínio

## Objetivo

Registrar pergunta real surgida de nota, fonte ou reflexão do usuário.

## Quando usar

Use quando uma dúvida precisa ser acompanhada.

## Quando não usar

Não use quando a pergunta é genérica e não tem vínculo com conteúdo real.

## Entrada esperada

Pergunta, origem e domínio provável.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não criar perguntas fictícias.
- Diferenciar pergunta aberta de tarefa.
- Linkar origem.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Registrar pergunta real surgida de nota, fonte ou reflexão do usuário.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Pergunta, origem e domínio provável.

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
Pergunta registrada para revisão futura.
```

## Resultado esperado

Pergunta registrada para revisão futura.

## Arquivos que podem ser afetados

- `02-domains/[domínio]/questions/`

## Observações

Perguntas podem virar revisão ou pesquisa depois, com confirmação.
