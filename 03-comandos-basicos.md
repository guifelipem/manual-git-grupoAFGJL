
# Comandos Básicos do Git

## 🧰 Comandos Essenciais e Suas Funções

### `git init`
**Função:**  
Inicia um novo repositório Git no diretório atual.  
Cria uma pasta oculta chamada `.git` para armazenar o histórico de versões do projeto.

📌 **Use no início de um projeto para começar a usar o Git.**

---

### `git status`
**Função:**  
Mostra o estado atual dos arquivos no projeto:
- Quais arquivos foram modificados.
- Quais estão prontos para o commit.
- Quais ainda não foram adicionados à área de preparação.

📌 **Use para verificar o que está acontecendo com seus arquivos no Git.**

---

### `git add`
**Função:**  
Adiciona arquivos ou mudanças para a *staging area* (área de preparação).  
Os arquivos adicionados ficam prontos para serem salvos no próximo commit.

```bash
git add nome-do-arquivo
git add .   # Adiciona todos os arquivos modificados
```

📌 **Use sempre que quiser salvar alguma modificação no histórico.**

---

### `git commit`
**Função:**  
Salva definitivamente no histórico do Git os arquivos que estão na área de preparação.  
É como tirar um “snapshot” (foto) do projeto naquele momento.

```bash
git commit -m "Mensagem explicando o que foi feito"
```

📌 **Use para registrar mudanças importantes no projeto.**

---

### `git log`
**Função:**  
Mostra o histórico de commits feitos no repositório:
- ID do commit
- Autor
- Data
- Mensagem

📌 **Use para acompanhar o que foi feito e quando.**

---

## 🔗 Dica Extra

Para simulações visuais e treinar comandos:
- [Learn Git Branching](https://learngitbranching.js.org)
- [GitSchool - Visualizing Git](https://git-school.github.io/visualizing-git/)
