# Criar template de e-mail

## Objetivo

Gerar modelo de e-mail reutilizável a partir de necessidade real do usuário.

## Quando usar

Use quando o usuário pedir um e-mail ou template.

## Quando não usar

Não use quando envolver fato não confirmado sobre pessoas ou empresas.

## Entrada esperada

Objetivo, público, tom e informações obrigatórias.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não inventar compromissos.
- Usar placeholders para dados variáveis.
- Manter clareza.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Gerar modelo de e-mail reutilizável a partir de necessidade real do usuário.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Objetivo, público, tom e informações obrigatórias.

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
Template de e-mail em `05-saidas/emails/` ou resposta no chat.
```

## Resultado esperado

Template de e-mail em `05-saidas/emails/` ou resposta no chat.

## Arquivos que podem ser afetados

- `05-saidas/emails/`

## Observações

Templates podem ter placeholders conceituais.
