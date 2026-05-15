# Captura rápida

## Objetivo

Converter uma ideia curta em uma entrada clara de captura, pronta para ficar em inbox.

## Quando usar

Use quando o usuário trouxer uma frase, pensamento ou ideia rápida.

## Quando não usar

Não use quando já houver fonte longa para processamento completo.

## Entrada esperada

Texto bruto da captura e, se houver, contexto mínimo fornecido pelo usuário.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Preservar a formulação original em uma seção própria.
- Não transformar em projeto ativo.
- Não criar wiki a partir de uma captura isolada.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Converter uma ideia curta em uma entrada clara de captura, pronta para ficar em inbox.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Texto bruto da captura e, se houver, contexto mínimo fornecido pelo usuário.

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
Uma entrada de captura limpa, com possíveis tags conceituais e próximos passos leves.
```

## Resultado esperado

Uma entrada de captura limpa, com possíveis tags conceituais e próximos passos leves.

## Arquivos que podem ser afetados

- `00-inbox/ ou inbox de área, se o usuário confirmar`

## Observações

A captura pode continuar incompleta; clareza não exige processamento final.
