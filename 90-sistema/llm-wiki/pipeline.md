# Pipeline da LLM Wiki

Fluxo principal:

`Capturar -> Classificar -> Processar -> Conectar -> Sintetizar -> Revisar -> Reutilizar`

## 1. Capturar

- Ideia solta entra em `00-inbox/`.
- Fonte externa entra em `01-fontes/inbox/`.

## 2. Classificar

A IA identifica tipo, area principal, areas secundarias, conceitos, entidades, perguntas e possiveis projetos.

## 3. Processar

A IA cria notas em `02-areas/` somente quando houver conteudo real.

## 4. Conectar

A IA usa `[[wikilinks]]` para conectar notas, conceitos, entidades, projetos, fontes e sinteses.

## 5. Sintetizar

Quando houver base real suficiente, a IA atualiza sinteses em `wiki/synthesis/`.

## 6. Revisar

A IA observa padroes, lacunas, perguntas abertas e fontes pendentes.

## 7. Reutilizar

O usuario consulta conhecimento organizado, revisoes e saidas finais.
