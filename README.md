![](/git_github2.png) 
# Documentação GIT
###### Este arquivo contém notas da aula 07, ministrada pelo Prof. [Francisco Walison](http://github.com/franciscowallison), em 09/06/23, no curso Desenvolvedor Full Stack da Digital College de Fortaleza/CE
## Objetivo.
    Este será um documento de ajuda para que o iniciante em programação possa entender as diferenças do GIT em relação ao GITHUB e também
    utilizar como fonte de consulta sempre que for necessário revisar ou relembrar os comandos mais utilizados do GIT. 

## O que é o GIT?
    O Git é um software que controla a versão e rastreia as alterações feitas em arquivos ao longo do tempo. 
    Com ele, é possível reverter um determinado arquivo para versões anteriores. Também será possível copiar um determinado arquivo e 
    fazer as alterações nesta cópia antes de mesclar as alterações ao arquivo original.
    
    Curiosidade! O Git não se limita a controlar alterações apenas em arquivos de código-fonte, ou seja, pode 
    ser usado para controlar a versão de qualquer tipo de arquivo, tais como arquivos de textos e até imagens

## O que é o GITHUB?
    É um serviço de hospedagem on-line para repositórios do Git que tem a capacidade de permitir a colaboração de 
    outros desenvolvedores de qualquer local.

## Pré-Requisitos
- Ter o GIT instalado na máquina. 
- Ter um editor de texto de sua escolha. Como sugestão, poderá baixar o [Visual Studio Code](https://code.visualstudio.com/download).
- Ter uma conta criada no [GitHub](https://github.com/).
- Configurar o sistema operacional para mostrar os arquivos ocultos (pasta .git).

## Como instalar o GIT
- Baixar a versão mais recente do [site oficial](https://git-scm.com/downloads). Neste momento tenha atenção para escolher a versão relativa ao seu sistema operacional nas opções fornecidas.

## Principais Comandos do GIT

#### Atribuir nome à sessão ativa:        
    git config --global user.name "<seu_nome>"
    
#### Atribuir email à sessão ativa:      
    git config --global user.email "<seu_email>"

#### Logar guardando sempre a senha:      
    git config --global credential.helper store

#### Criar uma nova branch ou ramo:
    git checkout -b <nome da branch>
        
####  Mudar de branch/ramo:
    git checkout <nome da branch>

#### Inicializa o arquivo ".git/" para controlar a pasta na máquina local que posteriormente subirá para o repositório do Github:
    git init: 

#### Clonar/baixar todo o projeto EXCLUSIVAMENTE do SEU repositório remoto informando o link do repositório que onde foi dado o fork e não do projeto original:
    git clone <url>

#### Validar os arquivos modificados dentro do projeto. (Em vermelho, ele mostra os arquivos modificados. Em verde, mostra os arquivos que foram adicionados pelo "git add"):
    git status
    
#### Adicionar todos os arquivos modificados na área segura antes do "commit": 
    git add .
    git add -A

#### Adicionar apenas um arquivo esepcificamente na área segura antes do "commit" 
    git add <nome do arquivo com a sua extensão>

#### Criar uma nova versão do projeto com as referências do criador:
    git commit -m "<texto_da_modificacao>"

#### Alterar o nome da branch principal de master para main (isso é uma boa prática atualmente recomendada)
    git branch -M "main" 

#### Passar o commit do repositório local (da minha máquina) para um repositório na plataforma do Github (Origin é o nome utilizado para referenciar o nosso repositório. Feito isto, o repositório local estará conectado com o respositório do Github, porém, o commit que damos na máquina não sobe automaticamente para a plataforma...)
    git remote add origin <link do repositório>

#### Subir, pela primeira vez, as alterações para o repositório remoto (github):
    git push -u origin <branch que quer subir (main ou develop, por ex)>
    
#### Subir, depois da primeira vez (sem o "-u", as alterações para o repositório remoto (github):
    git push origin <branch que quer subir (main ou develop, por ex)>

#### Puxar as alterações do repositório (quando trabalho no rep remoto e o aconteceram atualizações do time depois disto, antes de retomar o trabalho é necessário atualizar):
    git pull
    
#### Validar os meus comentários e modificações:
    git log

#### Adicionar o conteúdo da branch atual no contéudo de outra branch:
    git merge <nome_da_branch>

#### Mostrar as alterações feitas:
    gitk

#### Mostrar exatamente o que você alterou (e não apenas quais arquivos foram alterados):
    gitdiff

#### Para checar a versão do git instalada
    git -v

## Deu Erro? O que fazer?
- **Erro: 403** - Isto costuma acontecer muito caso o terminal GIT já se encontre ativado por outro usuário. É provavel que os usuários de GIT e GITHUB sejam diferentes.
  Neste caso, acessar o gerenciador de credenciais do windows e remover o usuário que estiver ativo no git resolerá o problema.
- **Erro: Remote origin already exists** - Isso provavelmente está acontecendo porque você já tinha feito envio para este repositório.Para ter certeza, execute o comando "git remote" e deve aparecer "origin", indicando que o repositório remoto já tinha sido configurado no Github. Neste caso, partir direto pro comando "git push -u origin master" ao inves de usar o "git remote add origin" utilizado na primeira vez.

## Dicas e Curiosidades
- Toda pasta com "." na frente do nome eh uma pasta oculta. 
- Caso ainda não esteja familiarizado em digitar a linha de comando no Git, você poderá abrir o Visual Code como editor e abrir o projeto nele primeiro. Feito isto, ao abrir o GIT o terminal já apontará para a linha de comando onde está o seu projeto.


## Referências
[Tutorial de Git e GitHub para iniciantes](https://www.freecodecamp.org/portuguese/news/tutorial-de-git-e-github-controle-de-versao-para-iniciantes/). 

[Templates para arquivos Readme](https://readme.so/pt/editor).

[Resolução do Erro 'remote origin already exits'](https://cursos.alura.com.br/forum/topico-erro-remote-origin-already-exists-o-que-fazer-14236).

