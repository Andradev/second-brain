# Atualizar índice de área

## Objetivo

Atualizar o `index.md` de uma área com links reais e estrutura legível.

## Quando usar

Use quando notas reais foram criadas, movidas ou revisadas na área.

## Quando não usar

Não use quando não houve alteração real na área.

## Entrada esperada

Área, arquivos relevantes e mudança ocorrida.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não linkar páginas inexistentes como se fossem reais.
- Manter o índice navegável.
- Registrar apenas conteúdo existente.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Atualizar o `index.md` de uma área com links reais e estrutura legível.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Área, arquivos relevantes e mudança ocorrida.

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
Índice da área atualizado com links úteis.
```

## Resultado esperado

Índice da área atualizado com links úteis.

## Arquivos que podem ser afetados

- `02-areas/[area-principal]/README.md`

## Observações

Pode incluir seções vazias apenas como estrutura se forem placeholders claros.
