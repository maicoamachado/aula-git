# aula-git
Aula GitHub - Code Education
Comandos github
:wq
//criar arquivos
touch arquivo

git log
git status
//adicionar um arquivo
git add arquivo
//adicionar todos os arquivos
git add .


//commits
git commit - m "descricao"
//Adicionar automaticamente os arquivos no momento do commit
git commit -a -m "descricao"

//listagem
git log --pretty=format: "%h -%an, %ar : %s"
git log --pretty=oneline
//detalhamento completo dos commits
git log -p

//ignorar arquivos
.gitignore

//Remover arquivo do git add
git reset HEAD arquivo

//voltar versao de acordo com o numero
git reset HEAD~1
git reset HEAD~2 --soft

//remove o arquivo commit permanente
git reset HEAD~1 --hard

//Fazer o conteúdo do arquivo voltar ao estado original
git checkout -- exemplo.php
//voltar para uma versão específica
git checkout hash

//Branches - Galhos
//visualizar branches
git branch
//criar branch
git checkout -b 'nome'
//voltar para um branch
git checkout nomebranch

//mesclar branches
 git merge nomebranch
//mesclar localmente reordernar
git rebase nomebranch
//Para remover um branch 
git branch -D nome-do-branch

//gerar chave github
ssh-keygen

//diretorio github
git remote add origin https://github.com/maicoamachado/aula-git.git
//fazendo o puch
git push origin master

//clonando
git clone
git clone checkout -b nomebranch origin/nomebranch
git branch -a

//para que possamos remover um branch remoto. Utilize o comando:

git push origin :nome-do-branch
