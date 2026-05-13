# Classificar ideia solta

## Objetivo

Sugerir a melhor categoria para uma ideia solta dentro do Second Brain.

## Quando usar

Use quando o usuário não souber onde colocar uma ideia.

## Quando não usar

Não use quando a ideia já for uma fonte bruta clara ou um projeto confirmado.

## Entrada esperada

Texto da ideia e qualquer contexto adicional fornecido.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Sugerir 2 ou 3 destinos prováveis se houver ambiguidade.
- Não mover arquivos sem autorização.
- Não criar projeto ativo automaticamente.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Sugerir a melhor categoria para uma ideia solta dentro do Second Brain.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Texto da ideia e qualquer contexto adicional fornecido.

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
Classificação sugerida com justificativa breve e próximo passo recomendado.
```

## Resultado esperado

Classificação sugerida com justificativa breve e próximo passo recomendado.

## Arquivos que podem ser afetados

- `00-inbox/`
- `02-domains/[domínio]/inbox/`
- `05-projects/inbox/`

## Observações

Classificação pode ser provisória.
