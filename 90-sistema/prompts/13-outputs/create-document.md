# Criar documento

## Objetivo

Gerar documento final a partir de notas, fontes ou briefing real.

## Quando usar

Use quando o usuário pedir um material final.

## Quando não usar

Não use quando ainda falta base ou objetivo claro.

## Entrada esperada

Objetivo do documento, público, fontes e formato.

## Regras importantes

- Não criar conteúdo simulado.
- Não inventar informações ausentes.
- Não apagar conteúdo real.
- Respeitar a estrutura do Second Brain.
- Verificar branch e `git status` quando houver alteração real.
- Não fazer merge automático.
- Não inventar base factual.
- Citar ou linkar origem interna quando útil.
- Salvar em `05-saidas/documentos/` se autorizado.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Gerar documento final a partir de notas, fontes ou briefing real.

Contexto:
Esta tarefa deve respeitar as regras do vault, preservar fontes originais, evitar conteúdo simulado e manter a main limpa.

Entrada esperada:
Objetivo do documento, público, fontes e formato.

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
Documento final em `05-saidas/documentos/`.
```

## Resultado esperado

Documento final em `05-saidas/documentos/`.

## Arquivos que podem ser afetados

- `05-saidas/documentos/`

## Observações

Documento final não substitui fonte original.
