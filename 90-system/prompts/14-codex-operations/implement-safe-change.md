# Implementar mudança segura

## Objetivo

Orientar o Codex a implementar uma mudança pequena ou média com validação.

## Quando usar

Use quando o usuário pedir alteração em arquivos do vault.

## Quando não usar

Não use quando a mudança exigir aprovação estrutural ainda não dada.

## Entrada esperada

Objetivo, arquivos permitidos e critérios de sucesso.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Verificar branch/status.
- Editar somente o escopo.
- Validar e resumir.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Orientar o Codex a implementar uma mudança pequena ou média com validação.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Objetivo, arquivos permitidos e critérios de sucesso.

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
Mudança implementada com segurança.
```

## Resultado esperado

Mudança implementada com segurança.

## Arquivos que podem ser afetados

- Arquivos indicados pelo usuário

## Observações

Se o escopo crescer, parar e pedir confirmação.
