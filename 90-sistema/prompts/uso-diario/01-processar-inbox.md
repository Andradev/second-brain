# Processar 00-inbox

## Objetivo

Organizar as ideias, dúvidas, tarefas soltas, pensamentos e anotações rápidas que estão em `00-inbox/`.

## Quando usar

Use este prompt quando você jogou várias coisas no `00-inbox/` e quer que a IA organize.

## Prompt copiável

```txt
Você é um agente de IA atuando no meu Second Brain Universal.

Objetivo:
Processar o conteúdo real que está em 00-inbox/.

Contexto:
O 00-inbox/ é a entrada principal para tudo que veio da minha cabeça, como ideias soltas, dúvidas, pensamentos, tarefas jogadas, anotações rápidas, reflexões e observações bagunçadas.

Regras:
1. Não criar conteúdo simulado.
2. Não inventar informações.
3. Não apagar conteúdo real.
4. Não criar projeto ativo sem minha confirmação.
5. Não executar automações.
6. Não fazer merge automático.
7. Preservar o que for incerto.
8. Usar a estrutura simplificada do Second Brain.
9. Usar o LLM Wiki interno em 90-sistema/llm-wiki/ apenas se houver conceito, entidade, pergunta, comparação ou síntese real suficiente.

Tarefas:
1. Ler o conteúdo real em 00-inbox/.
2. Identificar o tipo de cada entrada.
3. Classificar cada entrada no local correto.

Critérios de classificação:

- Ideias organizadas devem ir para:
  02-areas/ideias/

- Coisas de trabalho devem ir para:
  02-areas/trabalho/

- Tarefas do trabalho devem ir para:
  02-areas/trabalho/tarefas/

- Dúvidas do trabalho devem ir para:
  02-areas/trabalho/duvidas/

- Regras de negócio devem ir para:
  02-areas/trabalho/regras-de-negocio/

- Processos da empresa devem ir para:
  02-areas/trabalho/processos/

- Estudos e aprendizados devem ir para:
  02-areas/estudos/

- Reflexões de fé, Bíblia, devocionais ou valores devem ir para:
  02-areas/fe-e-valores/

- Coisas de vida pessoal devem ir para:
  02-areas/vida-pessoal/

- Ideias quase prontas para virar projeto devem ir para:
  03-projetos/inbox/

4. Se algo ainda estiver confuso, manter em 00-inbox/ ou mover para 00-inbox/para-processar/.
5. Criar links internos quando fizer sentido.
6. Atualizar índices necessários, se existirem.
7. Atualizar logs necessários, se existirem.
8. Se houver conhecimento recorrente real, atualizar o LLM Wiki interno em:
   90-sistema/llm-wiki/
9. Ao final, responder com um resumo do que foi feito.

Resultado esperado:
O 00-inbox/ fica mais organizado, sem perda de informação, e o conteúdo é distribuído para as áreas corretas.
```

## Resultado esperado

Depois de usar este prompt, o conteúdo solto do 00-inbox/ deve ser classificado e organizado nas áreas certas.
