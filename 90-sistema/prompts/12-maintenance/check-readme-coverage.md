# Verificar cobertura de README

## Objetivo

Verificar se pastas importantes têm README explicativo.

## Quando usar

Use quando novas pastas forem criadas.

## Quando não usar

Não use quando a pasta é temporária e não precisa documentação.

## Entrada esperada

Escopo de pastas.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não criar documentação falsa.
- Usar descrição operacional, não conteúdo real.
- Manter README curto.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Verificar se pastas importantes têm README explicativo.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Escopo de pastas.

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
Lista de pastas sem README ou READMEs criados com segurança.
```

## Resultado esperado

Lista de pastas sem README ou READMEs criados com segurança.

## Arquivos que podem ser afetados

- Qualquer pasta estrutural do vault

## Observações

READMEs documentam função da pasta, não preenchem conhecimento.
