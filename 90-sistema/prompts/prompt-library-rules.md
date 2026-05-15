# Regras da Biblioteca de Prompts

## 1. Prompts são modelos, não execuções

Arquivos dentro de `90-sistema/prompts/` são modelos reutilizáveis.

Eles não devem ser executados automaticamente apenas por existirem.

## 2. Não criar conteúdo simulado

Nenhum prompt deve criar arquivos reais com base em exemplos conceituais.

Exemplos dentro dos prompts servem apenas para explicar o uso.

## 3. Main limpa

Prompts que alteram conteúdo real devem recomendar branch separada.

A branch `main` deve permanecer como template limpo.

## 4. Confirmação humana

Mudanças estruturais médias ou grandes exigem confirmação humana.

## 5. Escopo limitado

Cada prompt deve executar uma tarefa clara.

Evitar prompts genéricos demais que tentem reorganizar o vault inteiro sem necessidade.

## 6. Segurança antes de execução

Prompts operacionais devem começar verificando:

- branch atual
- git status
- escopo da tarefa
- risco de apagar conteúdo real

## 7. Não fazer merge automático

Nenhum prompt deve fazer merge automático na main.

## 8. Não apagar conteúdo real

Se houver dúvida, mover para 99-arquivo/revisar.

## 9. Separação entre prompt e resultado

O prompt fica em `90-sistema/prompts/`.

O resultado gerado pelo prompt deve ir para a área correta do vault.

## 10. Prompts devem ser claros

Cada prompt deve explicar:

- objetivo
- quando usar
- quando não usar
- entrada esperada
- regras
- passos
- resultado esperado
