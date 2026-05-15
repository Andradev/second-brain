# Manter main como template limpo

## Objetivo

Orientar manutenção da main como estrutura base sem conteúdo processado indevido.

## Quando usar

Use quando revisar estado da main ou preparar template.

## Quando não usar

Não use quando estiver em branch de conteúdo.

## Entrada esperada

Objetivo da limpeza e status da branch.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não apagar conteúdo real sem pedido.
- Não fazer merge automático.
- Separar template de conteúdo.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Orientar manutenção da main como estrutura base sem conteúdo processado indevido.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Objetivo da limpeza e status da branch.

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
Main ou branch de template avaliada com segurança.
```

## Resultado esperado

Main ou branch de template avaliada com segurança.

## Arquivos que podem ser afetados

- `Git`
- `README.md`
- `90-sistema/`

## Observações

Esse prompt é sensível e deve pedir confirmação antes de limpezas.
