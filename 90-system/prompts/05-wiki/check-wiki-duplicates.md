# Verificar duplicidades na wiki

## Objetivo

Encontrar possíveis conceitos, entidades ou sínteses duplicadas.

## Quando usar

Use quando a wiki crescer ou parecer inconsistente.

## Quando não usar

Não use quando o objetivo for reescrever conteúdo sem revisão.

## Entrada esperada

Escopo da verificação na wiki.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não mesclar automaticamente sem confirmação.
- Preservar conteúdo real.
- Sugerir unificação com justificativa.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Encontrar possíveis conceitos, entidades ou sínteses duplicadas.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Escopo da verificação na wiki.

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
Lista de possíveis duplicidades e recomendação.
```

## Resultado esperado

Lista de possíveis duplicidades e recomendação.

## Arquivos que podem ser afetados

- `03-wiki/concepts/`
- `03-wiki/entities/`
- `03-wiki/synthesis/`

## Observações

Duplicidade provável não é certeza; revisar antes de mover.
