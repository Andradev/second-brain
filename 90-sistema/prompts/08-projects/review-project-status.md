# Revisar status do projeto

## Objetivo

Revisar andamento de projeto ativo com base em arquivos reais.

## Quando usar

Use quando o usuário pedir revisão de projeto.

## Quando não usar

Não use quando o projeto não existe ou não foi confirmado.

## Entrada esperada

Projeto e período de revisão.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Analisar contexto, tarefas e decisões.
- Não alterar escopo sem confirmação.
- Sugerir próximos passos.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Revisar andamento de projeto ativo com base em arquivos reais.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Projeto e período de revisão.

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
Revisão clara do status do projeto.
```

## Resultado esperado

Revisão clara do status do projeto.

## Arquivos que podem ser afetados

- `03-projetos/ativos/[projeto]/`
- `04-revisoes/`

## Observações

A revisão pode gerar recomendações, mas não executa tudo sozinha.
