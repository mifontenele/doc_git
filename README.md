###### (Este arquivo contém notas da aula 07, ministrada pelo Prof. Francisco Walison (http://github.com.br/franciscowallison), em 09/06/23, no curso Desenvolvedor Full Stack da Digital College de Fortaleza/CE)

# Documentação GIT

## Objetivo
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
    1. Ter o GIT instalado na máquina. 
    2. Ter um editor de texto de sua escolha. Como sugestão, poderá baixar o VISUAL STUDIO CODE disponível para 
    download no endereço https://code.visualstudio.com/download.
    3. Ter uma conta criada no GITHUB. Download disponível no link https://github.com/.
    4. Configurar o sistema operacional para mostrar os arquivos ocultos (pasta .git).

## Como instalar o GIT
    Baixar a versão mais recente do site oficial disponível através do link https://git-scm.com/downloads. 
    Neste momento tenha atenção para escolher a versão relativa ao seu sistema operacional nas opções 
    fornecidas.

## Principais Comandos do GIT

#### Atribuir nome à sessão ativa:        
`Use git config --global user.name "<seu_nome>" para atribuir'

#### Atribuir email à sessão ativa:      
    git config --global user.email "<seu_email>"

#### Criar uma nova branch ou ramo:
    git checkout -b <nome da branch>
        
####  Mudar de branch/ramo:
    git checkout <nome da branch>

#### Iniciar o arquivo ".git/" para controlar a pasta:
    git init: 

#### Validar os arquivos modificados dentro do projeto. Em vermelho, ele mostra os arquivos modificados. Em verde, mostra os arquivos que foram adicionados pelo "git add":
    git status
    
#### Colocar o arquivo modificado em uma área segura: 
    git add

#### Criar uma nova versão do projeto com as referências do criador:
    git commit -m "<texto_da_modificacao>"

#### Clonar/baixar todo o projeto do repositório remoto (link do repositório informado):
    git clone <url>

#### Subir as alterações para o repositório remoto (github):
    git push

#### Puxar as alterações do repositório:
    git pull
    
#### Validar os meus comentários e modificações:
    git log

#### Adicionar o conteúdo da branch atual no contéudo de outra branch:
    git merge <nome_da_branch>

#### Mostrar as alterações feitas:
    gitk

## Deu Erro? O que fazer?
        
    Erro: 403
    Isto costuma acontecer muito caso o terminal GIT já se encontre ativado por outro usuário. É provavel que os usuários de GIT e GITHUB sejam diferentes. Neste caso, acessar o gerenciador de credenciais do windows e remover o usuário que estiver ativo no git resolerá o problema.

    Erro: Remote origin already exists
    Isso provavelmente está acontecendo porque você já tinha feito envio para este repositório.Para ter certeza, execute o comando "git remote" e deve aparecer "origin", indicando que o repositório remoto já tinha sido configurado no Github. Neste caso, partir direto pro comando "git push -u origin master" ao inves de usar o "git remote add origin" utilizado na primeira vez.

## Dicas e Curiosidades
    Toda pasta com "." na frente do nome eh uma pasta oculta. 
    
    Caso ainda não esteja familiarizado em digitar a linha de comando no Git, você poderá abrir o Visual Code como editor e abrir o projeto nele primeiro. Feito isto, ao abrir o GIT o terminal já apontará para a linha de comando onde está o seu projeto.

    Para checar a versão do git instalada
    git -v

## Referência
    https://www.freecodecamp.org/portuguese/news/tutorial-de-git-e-github-controle-de-versao-para-iniciantes/
    
    https://readme.so/pt/editor

    https://cursos.alura.com.br/forum/topico-erro-remote-origin-already-exists-o-que-fazer-14236
