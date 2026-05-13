# Processar fonte específica

## Objetivo

Processar uma fonte bruta específica e criar notas derivadas no local correto.

## Quando usar

Use quando o usuário indicar uma fonte real para processar.

## Quando não usar

Não use quando a fonte for apenas exemplo de template ou não existir no vault.

## Entrada esperada

Caminho da fonte, tipo, domínio provável e objetivo do processamento.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Preservar fonte original.
- Criar conteúdo apenas a partir da fonte.
- Registrar fonte usada.
- Mover para `processed/` da própria categoria ao final, se autorizado.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Processar uma fonte bruta específica e criar notas derivadas no local correto.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Caminho da fonte, tipo, domínio provável e objetivo do processamento.

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
Fonte processada em nota de domínio, com links e pendências reais.
```

## Resultado esperado

Fonte processada em nota de domínio, com links e pendências reais.

## Arquivos que podem ser afetados

- `01-raw/[categoria]/`
- `02-domains/[domínio]/sources/`
- `02-domains/[domínio]/notes/`
- `03-wiki/`

## Observações

Se a fonte tocar múltiplos domínios, escolha um principal e crie links cruzados.
