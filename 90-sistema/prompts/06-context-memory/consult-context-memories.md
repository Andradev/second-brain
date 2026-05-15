# Consultar memórias contextuais

## Objetivo

Consultar memórias relevantes antes de responder ou operar em um assunto.

## Quando usar

Use quando uma tarefa toca domínio, projeto ou assunto com possíveis memórias.

## Quando não usar

Não use quando a pergunta é totalmente fora do vault e sem contexto recorrente.

## Entrada esperada

Tema da tarefa e domínio provável.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Ler memórias relevantes.
- Aplicar apenas as que realmente se conectam ao tema.
- Não inventar memória ausente.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Consultar memórias relevantes antes de responder ou operar em um assunto.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Tema da tarefa e domínio provável.

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
Resposta ou ação considera memórias existentes.
```

## Resultado esperado

Resposta ou ação considera memórias existentes.

## Arquivos que podem ser afetados

- `02-areas/[domínio]/memory/`

## Observações

Se não houver memória, diga isso de forma simples quando relevante.
