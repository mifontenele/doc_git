# Documentação git
Documentação de ajuda nos comando git


CONFIGURAÇÃO DO USUÁRIO NO GIT:
git config --global user.name "<seu_nome>"
git config --global user.email "<seu_email>"

git init: Ele inicia o arquivo ".git/" para controlar a pasta. (toda pasta com "." na frente do ome eh uma pasta oculta)

git status: responsanvel por valida os arquivos modificados dentro do projeto. 
Em vermelho ele mostra os arquivos modificados. 
Em verde mostra os arquivos que foram adicionados pelo "git add"

git add: responsável por colocar o arquivo modificado em uma area segura (depois de digitar o arquivo identificado pelo git status em vermelho, o git add adiciona o arquivo e ao darmos GIT STATUS novamente o arquivo já aparece em verde.)

git commit -m "<texto_da_modificacao>": ele é responsável por criar uma nova versão do projeto com as referencias do criador.

git log: validar os meus comentários e modificações              

git checkout -b <nome da branch>: cria uma nova branch ou ramo

git checkout <nome da branch>: muda de branch/ ramo

git merge <nome_da_branch>: Ele adiciona a branch atual no contéudo de outra branch

gitk: mostra tudo que foi feito

git clone <url>: clona/baixa todo o projeto do repositório (link informado). 

git push: sobe as alterações para o repositório remoto (github)

git pull: Ele puxa as alteraões do repositório.

Erro 403: limpar as credenciais do windows
