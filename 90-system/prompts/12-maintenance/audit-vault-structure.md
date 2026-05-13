# Auditar estrutura do vault

## Objetivo

Verificar se as pastas principais e módulos seguem o padrão do Second Brain.

## Quando usar

Use quando houver suspeita de desorganização estrutural.

## Quando não usar

Não use quando o usuário pediu processamento de conteúdo específico.

## Entrada esperada

Escopo da auditoria.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não mover arquivos nessa etapa sem confirmação.
- Distinguir erro real de variação aceitável.
- Listar achados.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Verificar se as pastas principais e módulos seguem o padrão do Second Brain.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Escopo da auditoria.

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
Relatório de auditoria estrutural com recomendações.
```

## Resultado esperado

Relatório de auditoria estrutural com recomendações.

## Arquivos que podem ser afetados

- Todo o vault, conforme escopo

## Observações

Auditoria pode virar proposta de evolução.
