# Processar artigo

## Objetivo

Processar um artigo real preservando a fonte e extraindo ideias úteis.

## Quando usar

Use quando houver artigo salvo, recorte, link com conteúdo disponível ou texto fornecido.

## Quando não usar

Não use quando o usuário trouxer apenas uma opinião sem fonte.

## Entrada esperada

Caminho ou conteúdo do artigo e domínio provável.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não inventar argumentos do autor.
- Distinguir resumo de interpretação.
- Criar wiki apenas se houver conceito real relevante.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Processar um artigo real preservando a fonte e extraindo ideias úteis.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Caminho ou conteúdo do artigo e domínio provável.

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
Artigo vira nota processada com ideias, conceitos e pendências.
```

## Resultado esperado

Artigo vira nota processada com ideias, conceitos e pendências.

## Arquivos que podem ser afetados

- `01-raw/articles/`
- `02-domains/[domínio]/sources/`
- `03-wiki/concepts/`

## Observações

Quando o artigo for externo, preservar metadados disponíveis.
