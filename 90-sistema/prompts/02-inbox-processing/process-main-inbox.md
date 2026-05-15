# Processar inbox principal

## Objetivo

Processar itens reais de `00-inbox/` e encaminhar cada um para o destino adequado.

## Quando usar

Use quando houver capturas reais em `00-inbox/`.

## Quando não usar

Não use quando o usuário pediu apenas auditoria ou leitura sem alterações.

## Entrada esperada

Lista de arquivos ou escopo dentro de `00-inbox/`.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Ler cada item antes de classificar.
- Não criar projeto ativo automaticamente.
- Registrar dúvidas quando surgirem de conteúdo real.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Processar itens reais de `00-inbox/` e encaminhar cada um para o destino adequado.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Lista de arquivos ou escopo dentro de `00-inbox/`.

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
Itens classificados, preservados e movidos ou transformados conforme autorização.
```

## Resultado esperado

Itens classificados, preservados e movidos ou transformados conforme autorização.

## Arquivos que podem ser afetados

- `00-inbox/`
- `02-areas/`
- `03-projetos/inbox/`
- `99-arquivo/revisar/`

## Observações

Não processe todo o vault se o escopo for uma pasta ou arquivo específico.
