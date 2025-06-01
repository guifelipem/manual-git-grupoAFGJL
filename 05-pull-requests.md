
# GitHub e Pull Requests

## Criar conta no GitHub

1. Acesse [github.com](https://github.com).
2. Clique em "Sign up" no canto superior direito.
3. Preencha o formulário com seu e-mail, senha e nome de usuário.
4. Siga as instruções para verificar seu e-mail.
5. Complete o processo de configuração do perfil.

## Criar repositório remoto
1. No GitHub, clique no ícone "+" no canto superior direito e selecione "New repository".
2. Dê um nome ao repositório e adicione uma descrição opcional.
3. Escolha se o repositório será público ou privado.
4. Marque a opção "Initialize this repository with a README" se desejar.
5. Clique em "Create repository".
6. Após criar, você verá instruções para clonar o repositório ou adicionar arquivos.
## Clonar, push, pull
### Clonar um repositório remoto
1. No repositório remoto, clique no botão "Code" e copie a URL do repositório.
2. Abra o terminal ou prompt de comando.
3. Navegue até o diretório onde deseja clonar o repositório.
4. Execute o comando:
   ```bash
   git clone <URL_DO_REPOSITORIO>
   ```
5. O repositório será clonado para o seu diretório local.
### Fazer push de alterações
1. Navegue até o diretório do repositório clonado.
2. Faça as alterações desejadas nos arquivos.
3. Adicione os arquivos alterados ao staging area:
   ```bash
   git add .
   ```
4. Faça um commit das alterações:
   ```bash
   git commit -m "Sua mensagem de commit"
   ```
5. Envie as alterações para o repositório remoto:
   ```bash
   git push origin main
   ```
### Fazer pull de alterações
1. Navegue até o diretório do repositório clonado.
2. Para atualizar seu repositório local com as últimas alterações do remoto, execute:
   ```bash
   git pull origin main
   ```
3. Isso irá baixar e integrar as alterações do repositório remoto ao seu repositório local.
## Pull requests e revisão de código
### Criar um Pull Request
1. Após fazer push de suas alterações para o repositório remoto, vá até a página do repositório no GitHub.
2. Clique na aba "Pull requests".
3. Clique no botão "New pull request".
4. Selecione a branch que contém suas alterações e a branch base (geralmente `main`).
5. Adicione um título e uma descrição para o pull request.
6. Clique em "Create pull request".
### Revisão de Código
1. Outros colaboradores podem revisar o pull request, comentando sobre as alterações.
2. Você pode responder aos comentários e fazer alterações adicionais.
3. Após as revisões, se tudo estiver correto, o pull request pode ser mesclado (merged) na branch base.
4. Para mesclar, clique no botão "Merge pull request" e confirme a ação.
### Fechar um Pull Request
1. Se você decidir não prosseguir com o pull request, pode fechá-lo sem mesclar.
2. Vá até o pull request e clique no botão "Close pull request".
3. Isso não excluirá as alterações, apenas encerrará a discussão sobre elas.
### Dicas para Pull Requests
- Mantenha os pull requests pequenos e focados em uma única tarefa ou correção.
- Escreva mensagens de commit claras e descritivas.
- Use comentários para explicar partes complexas do código.
- Revise o código de outros colaboradores com atenção e respeito.
### Resolvendo Conflitos de Merge
- Se houver conflitos ao tentar mesclar um pull request, o GitHub indicará quais arquivos estão em conflito.
- Você precisará resolver esses conflitos manualmente.
- Abra os arquivos em conflito, localize as seções conflitantes e decida qual versão manter.
- Após resolver os conflitos, adicione os arquivos alterados ao staging area e faça um novo commit.
- Em seguida, faça push das alterações para o repositório remoto.
- O pull request será atualizado automaticamente com as alterações resolvidas.
### Conclusão
Pull requests são uma parte essencial do fluxo de trabalho colaborativo no GitHub. Eles permitem que os desenvolvedores proponham alterações, revisem o código de outros e integrem melhorias de forma organizada. Ao seguir as práticas recomendadas, você pode contribuir efetivamente para projetos e melhorar a qualidade do código em equipe.    

### Conclusão

Pull requests facilitam o trabalho em equipe no GitHub, permitindo propor, revisar e integrar alterações de forma organizada. Seguindo boas práticas, todos podem colaborar e melhorar o projeto juntos.    
