# Processar inbox de domínio

## Objetivo

Processar entradas reais dentro do inbox de um domínio específico.

## Quando usar

Use quando um domínio tiver capturas em `02-domains/[domínio]/inbox/`.

## Quando não usar

Não use quando o domínio não tiver manual ou o escopo for incerto demais sem confirmação.

## Entrada esperada

Nome do domínio e arquivos do inbox a processar.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Ler `_manual.md` do domínio antes.
- Criar nota processada somente com base no conteúdo real.
- Atualizar index/log quando houver processamento real.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Processar entradas reais dentro do inbox de um domínio específico.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Nome do domínio e arquivos do inbox a processar.

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
Entradas do domínio viram notas, perguntas ou pendências reais.
```

## Resultado esperado

Entradas do domínio viram notas, perguntas ou pendências reais.

## Arquivos que podem ser afetados

- `02-domains/[domínio]/inbox/`
- `02-domains/[domínio]/notes/`
- `02-domains/[domínio]/log.md`

## Observações

Memórias só podem ser criadas se o usuário pedir ou houver regra explícita.
