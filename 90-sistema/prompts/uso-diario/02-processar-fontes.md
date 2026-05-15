# Processar 01-fontes/inbox

## Objetivo

Classificar e processar fontes externas adicionadas em 01-fontes/inbox/.

## Quando usar

Use este prompt quando você adicionou vídeos, artigos, PDFs, aulas, prints, documentos, transcrições ou materiais externos em 01-fontes/inbox/.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Classificar e processar as fontes reais que estão em 01-fontes/inbox/.

Contexto:
A pasta 01-fontes/inbox/ guarda conteúdos que vieram de fora, como vídeos, artigos, PDFs, aulas, prints, documentos, transcrições, livros, documentações da empresa e materiais de referência.

Regras:
1. Preservar a fonte original.
2. Não inventar informação.
3. Não criar conteúdo simulado.
4. Não apagar conteúdo real.
5. Não criar projeto ativo sem minha confirmação.
6. Não executar automações.
7. Não fazer merge automático.
8. Se houver dúvida, manter em 01-fontes/inbox/ ou mover para 99-arquivo/revisar/.
9. Usar o LLM Wiki interno em 90-sistema/llm-wiki/ apenas quando houver conteúdo real suficiente.

Tarefas:
1. Ler as fontes reais em 01-fontes/inbox/.
2. Identificar o tipo de cada fonte:
   - vídeo
   - artigo
   - PDF
   - aula
   - print
   - livro
   - documento de trabalho
   - documentação da empresa
   - transcrição
   - reunião
   - outro material de referência

3. Identificar a área principal da fonte:
   - trabalho
   - estudos
   - fé e valores
   - vida pessoal
   - ideias
   - projetos

4. Se a fonte for útil, criar uma nota organizada na área correta em 02-areas/.

Critérios de destino:

- Documento ou processo da empresa:
  02-areas/trabalho/processos/

- Regra de negócio:
  02-areas/trabalho/regras-de-negocio/

- Dúvida ou aprendizado técnico:
  02-areas/estudos/
  ou 02-areas/trabalho/duvidas/, se nasceu no contexto do trabalho

- Conteúdo de estudo:
  02-areas/estudos/

- Conteúdo espiritual, bíblico, devocional ou de valores:
  02-areas/fe-e-valores/

- Conteúdo de vida pessoal:
  02-areas/vida-pessoal/

- Conteúdo que gera ideia:
  02-areas/ideias/

5. Se a fonte gerar conhecimento recorrente real, atualizar o LLM Wiki interno em:
   90-sistema/llm-wiki/

Possíveis destinos no LLM Wiki interno:

- Conceitos:
  90-sistema/llm-wiki/wiki/concepts/

- Entidades:
  90-sistema/llm-wiki/wiki/entities/

- Sínteses:
  90-sistema/llm-wiki/wiki/synthesis/

- Perguntas abertas:
  90-sistema/llm-wiki/wiki/questions/

- Comparações:
  90-sistema/llm-wiki/wiki/comparisons/

- Fontes estruturadas:
  90-sistema/llm-wiki/wiki/sources/

6. Depois de processar uma fonte com segurança, mover a fonte original para:
   01-fontes/processadas/

7. Se a fonte não puder ser processada agora, manter em:
   01-fontes/inbox/

8. Se a fonte estiver duplicada, antiga ou incerta, mover para:
   99-arquivo/revisar/

9. Atualizar índices necessários, se existirem.
10. Atualizar logs necessários, se existirem.
11. Ao final, responder com um resumo do que foi feito.

Resultado esperado:
As fontes de 01-fontes/inbox/ são preservadas, classificadas e transformadas em notas organizadas, mantendo a base LLM Wiki interna atualizada quando fizer sentido.
```

## Resultado esperado

Depois de usar este prompt, as fontes externas devem ser processadas, preservadas e conectadas às áreas corretas e ao LLM Wiki interno quando fizer sentido.
