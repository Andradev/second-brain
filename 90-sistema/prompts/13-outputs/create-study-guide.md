# Criar guia de estudo

## Objetivo

Gerar guia de estudo com base em notas ou fontes reais.

## Quando usar

Use quando há material de estudo real.

## Quando não usar

Não use quando o tema não tem base no vault e o usuário não pediu criação livre.

## Entrada esperada

Tema, notas/fontes e nível desejado.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não inventar conteúdo da aula/fonte.
- Separar resumo, exercícios e dúvidas.
- Linkar origem.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Gerar guia de estudo com base em notas ou fontes reais.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Tema, notas/fontes e nível desejado.

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
Guia de estudo em `05-saidas/study-guides/`.
```

## Resultado esperado

Guia de estudo em `05-saidas/study-guides/`.

## Arquivos que podem ser afetados

- `05-saidas/study-guides/`

## Observações

Pode apontar lacunas para estudo futuro.
