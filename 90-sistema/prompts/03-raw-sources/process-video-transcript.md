# Processar transcrição de vídeo

## Objetivo

Transformar uma transcrição real de vídeo em nota processada e conhecimentos conectáveis.

## Quando usar

Use quando houver transcrição, resumo ou notas reais de um vídeo.

## Quando não usar

Não use quando só houver título ou intenção de assistir.

## Entrada esperada

Caminho da transcrição e dados básicos do vídeo, se disponíveis.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não inventar falas ou timestamps.
- Separar resumo, ideias, citações curtas e perguntas.
- Preservar fonte em `01-fontes/`.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Transformar uma transcrição real de vídeo em nota processada e conhecimentos conectáveis.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Caminho da transcrição e dados básicos do vídeo, se disponíveis.

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
Nota processada com aprendizados, conceitos reais e referência à fonte.
```

## Resultado esperado

Nota processada com aprendizados, conceitos reais e referência à fonte.

## Arquivos que podem ser afetados

- `01-fontes/`
- `01-fontes/`
- `02-areas/[area-principal]/`

## Observações

Citações devem ser curtas e fiéis ao texto fornecido.
