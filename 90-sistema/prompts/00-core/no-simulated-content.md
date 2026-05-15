# Impedir conteúdo simulado

## Objetivo

Orientar o agente a nunca criar arquivos reais, conceitos, entidades, projetos, fontes ou sínteses a partir de exemplos conceituais.

## Quando usar

Use quando uma tarefa envolver templates, prompts, manuais ou exemplos que poderiam ser confundidos com conteúdo real.

## Quando não usar

Não use quando o usuário fornecer uma fonte real e pedir explicitamente seu processamento.

## Entrada esperada

O texto da tarefa e qualquer exemplo ou template que precise ser protegido contra uso indevido.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Tratar exemplos como placeholders.
- Não criar notas reais a partir de exemplos.
- Se houver dúvida sobre a origem, pedir confirmação.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Orientar o agente a nunca criar arquivos reais, conceitos, entidades, projetos, fontes ou sínteses a partir de exemplos conceituais.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
O texto da tarefa e qualquer exemplo ou template que precise ser protegido contra uso indevido.

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
O agente executa a tarefa sem transformar exemplos em conteúdo do vault.
```

## Resultado esperado

O agente executa a tarefa sem transformar exemplos em conteúdo do vault.

## Arquivos que podem ser afetados

- Arquivos do escopo solicitado
- Nenhuma nota real deve ser criada a partir de exemplos

## Observações

Este prompt é uma trava de segurança conceitual.
