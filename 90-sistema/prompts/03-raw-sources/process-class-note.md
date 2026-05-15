# Processar nota de aula

## Objetivo

Transformar notas reais de aula em material organizado de estudo.

## Quando usar

Use quando houver anotações, slides ou transcrição de aula.

## Quando não usar

Não use quando a aula ainda não tiver conteúdo capturado.

## Entrada esperada

Caminho da nota de aula, curso ou tema, se fornecidos.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não completar aula com conhecimento externo sem pedido.
- Separar conteúdo ensinado de dúvidas do usuário.
- Registrar lacunas.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Transformar notas reais de aula em material organizado de estudo.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Caminho da nota de aula, curso ou tema, se fornecidos.

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
Nota de estudo organizada no domínio correto.
```

## Resultado esperado

Nota de estudo organizada no domínio correto.

## Arquivos que podem ser afetados

- `01-fontes/`
- `02-areas/estudos/`
- `02-areas/[domínio]/notes/`

## Observações

Pode gerar perguntas de estudo quando surgirem do conteúdo real.
