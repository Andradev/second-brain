# Atualizar índice da wiki

## Objetivo

Atualizar índices da wiki com páginas reais existentes.

## Quando usar

Use quando páginas de conceitos, entidades, sínteses ou perguntas mudarem.

## Quando não usar

Não use quando não houver mudança real na wiki.

## Entrada esperada

Categorias ou páginas alteradas.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não linkar arquivos inexistentes.
- Evitar duplicidade.
- Manter navegação clara.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Atualizar índices da wiki com páginas reais existentes.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Categorias ou páginas alteradas.

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
Índices da wiki atualizados.
```

## Resultado esperado

Índices da wiki atualizados.

## Arquivos que podem ser afetados

- `03-wiki/README.md`
- `03-wiki/*/README.md`

## Observações

Índices devem ajudar a encontrar conteúdo, não inflar estrutura.
