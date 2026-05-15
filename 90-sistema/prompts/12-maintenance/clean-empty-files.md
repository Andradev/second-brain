# Limpar arquivos vazios

## Objetivo

Identificar arquivos vazios ou placeholders sem conteúdo real.

## Quando usar

Use quando há suspeita de arquivos vazios desnecessários.

## Quando não usar

Não use quando arquivos vazios servem como placeholders estruturais úteis.

## Entrada esperada

Escopo e regra para placeholders.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não remover sem confirmar utilidade.
- Preservar README e placeholders necessários.
- Não apagar conteúdo real.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Identificar arquivos vazios ou placeholders sem conteúdo real.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Escopo e regra para placeholders.

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
Lista de arquivos vazios com ação recomendada.
```

## Resultado esperado

Lista de arquivos vazios com ação recomendada.

## Arquivos que podem ser afetados

- Todo o vault, conforme escopo

## Observações

Limpeza destrutiva exige confirmação.
