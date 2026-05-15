# Criar relatório

## Objetivo

Gerar relatório a partir de execução, análise ou conteúdo real.

## Quando usar

Use quando há dados, logs ou achados reais.

## Quando não usar

Não use quando seria um relatório fictício de execução não feita.

## Entrada esperada

Escopo, período e evidências.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Relatar somente o verificado.
- Separar achados de recomendações.
- Não fingir validações.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Gerar relatório a partir de execução, análise ou conteúdo real.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Escopo, período e evidências.

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
Relatório final em `05-saidas/relatorios/`.
```

## Resultado esperado

Relatório final em `05-saidas/relatorios/`.

## Arquivos que podem ser afetados

- `05-saidas/relatorios/`

## Observações

Se nada foi executado, não chame de relatório de execução.
