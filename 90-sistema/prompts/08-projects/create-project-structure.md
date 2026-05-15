# Criar estrutura de projeto

## Objetivo

Criar estrutura padrão para um projeto confirmado.

## Quando usar

Use quando há projeto ativo confirmado.

## Quando não usar

Não use quando é só uma ideia ou hipótese.

## Entrada esperada

Nome do projeto, objetivo, domínio e confirmação.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não criar conteúdo fictício.
- Usar templates existentes quando houver.
- Registrar decisões conhecidas.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Criar estrutura padrão para um projeto confirmado.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Nome do projeto, objetivo, domínio e confirmação.

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
Estrutura de projeto pronta para uso.
```

## Resultado esperado

Estrutura de projeto pronta para uso.

## Arquivos que podem ser afetados

- `03-projetos/ativos/[projeto]/`

## Observações

Estrutura vazia demais deve ser evitada; use placeholders claros quando necessário.
