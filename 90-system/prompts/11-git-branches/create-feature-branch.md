# Criar feature branch

## Objetivo

Criar uma branch de trabalho com nome claro e escopo definido.

## Quando usar

Use antes de mudança estrutural, processamento real ou automação.

## Quando não usar

Não use quando o usuário pediu apenas leitura.

## Entrada esperada

Tipo, descrição curta e data.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Verificar branch atual.
- Verificar alterações existentes.
- Não descartar nada.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Criar uma branch de trabalho com nome claro e escopo definido.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Tipo, descrição curta e data.

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
Branch criada ou recomendada com segurança.
```

## Resultado esperado

Branch criada ou recomendada com segurança.

## Arquivos que podem ser afetados

- `Git`

## Observações

Use prefixos como `feature/`, `content/`, `system/` ou outro padrão definido.
