# LLM Wiki interna

Esta pasta guarda o nucleo de conhecimento conectado do Second Brain.

Ela e usada pela IA, nao pelo usuario no uso diario.

## Logica

1. O usuario adiciona ideias em `00-inbox/` ou fontes em `01-fontes/`.
2. A IA processa fontes e notas quando solicitada.
3. A IA cria notas organizadas em `02-areas/`.
4. A IA atualiza a wiki interna com conceitos, entidades, sinteses, perguntas e comparacoes.
5. A wiki interna cresce ao longo do tempo como uma base persistente de conhecimento.

## Regra principal

A wiki interna nao deve conter conteudo simulado.

So criar paginas a partir de conteudo real, fonte real, pedido explicito do usuario ou conteudo ja existente no vault.

## Estrutura

- `pipeline.md`: fluxo de operacao da LLM Wiki.
- `index.md`: indice do nucleo interno.
- `log.md`: historico de atualizacoes de conhecimento.
- `wiki/concepts/`: conceitos recorrentes.
- `wiki/entities/`: entidades importantes.
- `wiki/sources/`: fontes processadas ou referenciadas.
- `wiki/synthesis/`: sinteses vivas.
- `wiki/comparisons/`: comparacoes.
- `wiki/questions/`: perguntas abertas.
