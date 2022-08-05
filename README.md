# Comandos Git

- `git config --global user.name "NOME"`: Configura o nome do usuário no "git local";
- `git config --global user.email "EMAIL"`: Configura o e-mail do usuário no "git local";
- `git config --list`: Lista as configurações disponíveis;
- `git init`: Inicia um repositório local;
- `git status`: Verifica o status dos arquivos;
- `git add "FILE_NAME" (ou "DIRECTORY_NAME")`: Adiciona um arquivo não rastreado ao stage;
- `git add --all (ou -A ou .)`: Adiciona todos os arquivos não rastreados ao stage;
- `git add -f "FILE_NAME"`: Força a adição de um arquivo presente no .gitignore;
- "`git commit -m "MESSAGE"`: Realiza o commit local dos arquivos que estava rastreados no stage;
- `git -a -m commit "MESSAGE"`: Adiciona todos os arquivos não rastreados para o stage e faz o commit local;
- `git commit --amend -m "NEW_MESSAGE"`: Faz alterações em um commit que ainda não foi mandado para o repositório remoto;
- `git log`: Exibe o histórico de versões;
- `git log --oneline`: Exibe o histórico de versões de maneira resumida;
- `git diff`: Mostra as modificações feitas nos arquivos em stage desde o último commit;
- `git checkout "FILE_NAME"`: Desfaz alterações em um arquivo que ainda não está em stage na branch;
- `git reset HEAD "FILE_NAME"`: Desfaz alterações em um arquivo que já está em stage;
- `git reset --hard`: Semelhante ao git checkout "FILE_NAME" porém desfaz as alterações em todos os arquivos que ainda não estão em stage naquela branch;
- `git reset --hard HEAD~NUMBER`: Volta alterações de NUMBER commits atrás;
- `git clean -f`: Desfaz (basicamente exclui) as alterações em arquivos não rastreados;
- `git clone INITIAL_PATH FINAL_PATH`: Clona o repositório de um repositório local "INITIAL_PATH" para o novo repositório local "FINAL_PATH";
- `git clone "URL"`: Clona o repositório remoto pra um repositório local;
- `git push`: Envia os commits feitos no local para o remoto;
- `git push -u origin "BRANCH_NAME"`: Deve ser usado para enviar os commits iniciais de cada repo local para o remoto;
- `git pull`: Faz a comparação entre os repo local e remote e baixa atualizações se necessário. Funciona fazendo um Fetch e um Merge;
- `git fetch`: Verifica se existe diferença entre o repo local e remoto;
- `git merge "BRANCH_NAME"`": Mescla a branch "BRANCH_NAME" na branch em que está;
- `git tag -a "TAG" HASH`: Adiciona uma tag personalizada "TAG" ao commit de hash HASH;
- `git tag -d "TAG"`: Delete tag;
- `git push origin --tags`: Faz o envio das tags do repo local para o remoto;
- `git branch`: Lista as branchs;
- `git checkout "BRANCH_NAME"`: Cria uma branch de nome "BRANCH_NAME";
- `git checkout -b "BRANCH_NAME"`: Cria uma branch de nome "BRANCH_NAME" e muda para ela;
- `git branch -m "NEW_BRANCH_NAME"`: Renomeia a branch que você está para "NEW_BRANCH_NAME";
- `git branch - "TARGET_BRANCH" "NEW_BRANCH_NAME"`: Renomeia a branch "TARGET_BRANCH" para "NEW_BRANCH_NAME";
- `git branch -d "BRANCH_NAME"`: Exclui localmente a branch "BRANCH_NAME" (não pode estar nela);
- `git branch -D "BRANCH_NAME"`: Força a exclusão local da branch "BRANCH_NAME";
- `git push origin --delete "BRANCH_NAME"`: Exclui a branch "BRANCH_NAME" no repo remoto;
- `git stash`: Salva temporariamente as alterações de arquivos;
- `git stash save "MESAGE"`: Salva temporariamente as alterações de arquivos, mas com uma mensgaem personalizada "MESSAGE";
- `git stash list`: Lista os 'stashes' feitos;
- `git stash apply`: Aplica o último stash feito;
- `git stash apply stash@{"NUMBER"}`: Aplica o stash de número "NUMBER";
- `git stash branch "BRANCH_NAME"`: Cria uma branch de nome "BRANCH_NAME" a partir de um stash;
- `git stash pop`: Aplica o último stash feito e o exclui da lista;
- `git stash pop stash@{"NUMBER"}`: Aplica o stash de número "NUMBER" e o exclui da lista;
- `git stash dropstash@{"NUMBER"}`: Dropa o stash de número "NUMBER" da lista de stashes;
- `git rebase "BRANCH_NAME"`: Faz a mesma coisa que o merge porém de um jeito diferente. Enquanto o 'merge' cria um commit e junta os existentes, já o 'rebase' joga os commits feitos na branch "BRANCH_NAME" na branch em que ele é feito;
- 2x 'esc' + `:wq` -> para salvar e sair do editor do git;




