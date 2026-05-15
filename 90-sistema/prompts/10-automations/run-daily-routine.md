# Rodar rotina diária

## Objetivo

Executar rotina diária documentada com segurança.

## Quando usar

Use quando o usuário pedir execução da rotina diária.

## Quando não usar

Não use quando estiver na main ou sem branch apropriada.

## Entrada esperada

Data, escopo e confirmação de execução.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Verificar branch.
- Não processar além do escopo.
- Gerar resumo do que mudou.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Executar rotina diária documentada com segurança.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Data, escopo e confirmação de execução.

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
Rotina diária concluída em branch separada.
```

## Resultado esperado

Rotina diária concluída em branch separada.

## Arquivos que podem ser afetados

- `00-inbox/`
- `04-revisoes/daily/`
- `90-sistema/automations/`

## Observações

Rotina não deve virar processamento total do vault.
