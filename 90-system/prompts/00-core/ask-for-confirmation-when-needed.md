# Pedir confirmação quando necessário

## Objetivo

Determinar quando uma mudança exige confirmação humana antes de continuar.

## Quando usar

Use quando a tarefa envolver reorganização, exclusão, criação de nova área, automação ou alteração em regras centrais.

## Quando não usar

Não use quando a mudança for pequena, reversível e explicitamente solicitada.

## Entrada esperada

Descrição da mudança pretendida e motivo da possível confirmação.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Pedir confirmação para mudanças estruturais médias ou grandes.
- Explicar impacto e arquivos afetados.
- Não prosseguir enquanto a confirmação não vier.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Determinar quando uma mudança exige confirmação humana antes de continuar.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Descrição da mudança pretendida e motivo da possível confirmação.

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
O agente identifica se deve parar para validação humana.
```

## Resultado esperado

O agente identifica se deve parar para validação humana.

## Arquivos que podem ser afetados

- Arquivos de sistema
- Pastas de domínio
- `AGENTS.md`
- `90-system/`

## Observações

Confirmação não é burocracia: é proteção contra reorganização indevida.
