# Classificar fontes do inbox

## Objetivo

Classificar fontes novas em `01-fontes/inbox/` sem criar varias pastas visiveis por tipo.

## Quando usar

Use quando houver fontes brutas pendentes e o usuario pedir organizacao ou revisao.

## Quando nao usar

Nao use para processar a fonte em nota final. Classificacao e diferente de processamento.

## Entrada esperada

Arquivos em `01-fontes/inbox/` ou lista de fontes.

## Regras importantes

- Nao criar conteudo simulado.
- Nao inventar informacoes ausentes.
- Nao apagar conteudo real.
- Nao editar a fonte original.
- Manter a fonte em `01-fontes/inbox/` se ela ainda nao foi processada.
- Usar metadados, tags ou anotacoes para registrar tipo e area provavel.
- Nao criar subpastas visiveis como `articles/`, `videos/` ou `work/`.

## Prompt copiavel

```txt
Voce e um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Classificar fontes novas em `01-fontes/inbox/` sem processar o conteudo ainda.

Tarefa:
1. Leia nomes, metadados e conteudo minimo necessario para entender cada fonte.
2. Identifique tipo de fonte, area provavel, assunto principal e duvidas.
3. Nao crie nota processada nesta etapa, salvo pedido explicito.
4. Nao crie conteudo simulado.
5. Preserve a fonte original.
6. Ao final, informe classificacao sugerida, pendencias e proximos passos.
```

## Resultado esperado

Fontes classificadas por tipo e area provavel, com duvidas preservadas.
