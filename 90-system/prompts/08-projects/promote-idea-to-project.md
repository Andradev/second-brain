# Promover ideia a projeto

## Objetivo

Transformar ideia em projeto ativo após confirmação explícita.

## Quando usar

Use quando o usuário confirmar que a ideia virou projeto.

## Quando não usar

Não use quando a confirmação não for clara.

## Entrada esperada

Ideia aprovada, nome do projeto e objetivo.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Exigir confirmação humana.
- Preservar origem da ideia.
- Criar estrutura mínima.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Transformar ideia em projeto ativo após confirmação explícita.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Ideia aprovada, nome do projeto e objetivo.

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
Projeto ativo criado com contexto inicial.
```

## Resultado esperado

Projeto ativo criado com contexto inicial.

## Arquivos que podem ser afetados

- `05-projects/active/`

## Observações

Promoção é uma mudança de status importante.
