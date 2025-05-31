# Branches e Merge

## O que são Branches?

Branches (ou ramificações) são uma funcionalidade essencial do Git que permite desenvolver funcionalidades de forma isolada do restante do código. Em vez de alterar diretamente a `main` (linha principal de desenvolvimento), criamos uma branch para fazer mudanças sem afetar o projeto principal.

Isso é útil para:

- Trabalhos em equipe paralelos
- Testes de novas funcionalidades
- Correção de bugs sem interromper o desenvolvimento principal

## Criar, Mudar e Deletar Branches

### Criar uma nova branch

```bash
git branch nome-da-branch
```

### Mudar para outra branch

```bash
git checkout nome-da-branch
```

> Dica: a partir do Git 2.23, o comando `git switch` também pode ser usado:

```bash
git switch nome-da-branch
```

### Criar e mudar para uma branch ao mesmo tempo

```bash
git checkout -b nome-da-branch
```

### Listar branches

```bash
git branch
```

### Deletar uma branch

```bash
git branch -d nome-da-branch
```

> Use `-D` (maiúsculo) para forçar a exclusão se necessário.

## Git Merge e Como Lidar com Conflitos

Após terminar o trabalho em uma branch, você pode mesclá-la (`merge`) com outra, geralmente a `main`.

### Fazer merge de uma branch

Primeiro, mude para a branch de destino (por exemplo, `main`):

```bash
git checkout main
```

Depois, faça o merge:

```bash
git merge nome-da-branch
```

### Conflitos de Merge

Quando duas branches modificam a mesma parte do código, ocorre um **conflito de merge**.

O Git avisará sobre os arquivos com conflitos. Você deve abrir esses arquivos, resolver manualmente os conflitos e depois adicionar e commitar:

```bash
git add nome-do-arquivo
git commit
```

Exemplo de conflito:

```plaintext
<<<<<<< HEAD
versão da main
=======
versão da branch
>>>>>>> nome-da-branch
```

Você deve escolher qual trecho manter (ou unir os dois de forma lógica) e salvar o arquivo.

## Demonstração Visual (Exemplo Simples)

