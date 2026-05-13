# Context Memories

## O que é este módulo

Context Memories são memórias recorrentes por assunto, domínio, projeto, tecnologia, pessoa ou situação.

Elas existem para guardar lembretes práticos que a IA deve considerar quando um contexto aparecer novamente.

## Para que serve

Use este módulo quando uma informação precisa ser lembrada de forma recorrente em futuras interações.

Context Memories podem guardar:

- Regras recorrentes de trabalho.
- Cuidados técnicos específicos.
- Preferências pessoais.
- Padrões que devem ser seguidos.
- Decisões já tomadas que afetam um assunto.
- Procedimentos repetitivos.
- Erros que não devem ser repetidos.
- Comandos importantes.
- Contextos que a IA deve considerar antes de responder.

## O que não é

Uma Context Memory não é uma nota comum, fonte bruta, tarefa ou projeto.

Ela é um lembrete persistente ligado a um contexto.

## Onde ficam as memórias

As memórias devem ser salvas no domínio mais relacionado:

```md
02-domains/[domínio]/memory/
```

## Arquivos deste módulo

- `context-memory-rules.md`: regras de criação, consulta e manutenção.
- `context-memory-template.md`: template para novas memórias contextuais.
- `examples.md`: exemplos conceituais de uso, sem criar memórias reais.

## Regra central

Não criar memórias fictícias.

Uma memória contextual só deve ser criada quando vier de informação real do usuário, conteúdo real existente no vault ou pedido explícito.
