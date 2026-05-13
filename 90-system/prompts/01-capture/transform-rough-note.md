# Transformar nota bruta

## Objetivo

Reorganizar uma nota solta em uma versão legível sem acrescentar informação externa.

## Quando usar

Use quando uma anotação do usuário estiver confusa, fragmentada ou misturar tópicos.

## Quando não usar

Não use quando a tarefa exigir pesquisa externa ou processamento de fonte bruta.

## Entrada esperada

Nota bruta escrita pelo usuário.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Separar fatos, ideias, dúvidas e ações.
- Sinalizar inferências claramente.
- Não criar arquivos finais sem confirmação.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Reorganizar uma nota solta em uma versão legível sem acrescentar informação externa.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Nota bruta escrita pelo usuário.

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
Nota reorganizada e preparada para classificação posterior.
```

## Resultado esperado

Nota reorganizada e preparada para classificação posterior.

## Arquivos que podem ser afetados

- `00-inbox/ ou 02-domains/[domínio]/inbox/`

## Observações

Use placeholders quando a nota ainda não tiver destino claro.
