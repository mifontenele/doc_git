(Este arquivo contém notas da aula 07, ministrada pelo Prof. Francisco Walison, em 09/06/23, no curso Desenvolvedor Full Stack da Digital College de Fortaleza/CE)

# Documentação GIT para Iniciantes

## Objetivo
    É comum ao iniciante pensar que GIT e GITHUB são a mesma coisa.
    Este será um documento de ajuda para que o iniciante em programação possa entender as diferenças do GIT em relação ao GITHUB e também utilizar como fonte de consulta sempre que for necessário revisar ou relembrar os comandos mais utilizados do GIT. 

## O que é o GIT?
    O Git é um software que controla a versão e rastreia as alterações feitas em arquivos ao longo do tempo. Com ele, é possível reverter um determinado arquivo para versões anteriores. Também será possível copiar um determinado arquivo e fazer as alterações nesta cópia antes de mesclar as alterações ao arquivo original.
    Curiosidade! O Git não se limita a controlar alterações apenas em arquivos de código-fonte, ou seja, pode ser usado para controlar a versão de qualquer tipo de arquivo, tais como arquivos de textos e até imagens

## O que é o GITHUB?
    É um serviço de hospedagem on-line para repositórios do Git que tem a capacidade de permitir a colaboração de outros desenvolvedores de qualquer local.

## Pré-Requisitos
    Ter o GIT instalado na máquina. 
    Ter um editor de texto de sua escolha. Como sugestão, poderá baixar o VISUAL STUDIO CODE disponível para download no endereço https://code.visualstudio.com/download.
    Ter uma conta criada no GITHUB. Download disponível no link https://github.com/.

## Como instalar o GIT
    Baixar a versão mais recente do site oficial disponível através do link https://git-scm.com/downloads. Neste momento tenha atenção para escolher a versão relativa ao seu sistema operacional nas opções fornecidas.

## Principais Comandos do GIT

Configuração de Usuário:
        
        git config --global user.name "<seu_nome>": 
        responsável por atribuir seu nome à sessão GIT ativa
        
        git config --global user.email "<seu_email>": 
        responsável por associar seu email à sessão GIT ativa

Iniciar:
        
        git init: 
        responsável por iniciar o arquivo ".git/" para controlar a pasta.
            Dica para o iniciante: Toda pasta com "." na frente do ome eh uma pasta oculta. caso ainda não esteja familiarizado em digitar a linha de comando no Git, você poderá abrir o Visual Code como editor e abrir o projeto nele primeiro. 
            Feito isto, ao abrir o GIT o terminal já apontará para a linha de comando onde está o seu projeto.

Principais Comandos:

        git status: 
        responsánvel por validar os arquivos modificados dentro do projeto. 
            Em vermelho, ele mostra os arquivos modificados. Em verde, mostra os arquivos que foram adicionados pelo "git add".

        git add:
        responsável por colocar o arquivo modificado em uma área segura 
            (depois de digitar o arquivo identificado pelo git status em vermelho, o git add adiciona o arquivo e ao darmos GIT STATUS novamente o arquivo já aparece em verde).

        git commit -m "<texto_da_modificacao>":
        responsável por criar uma nova versão do projeto com as referências do criador.

        git log:
        responsável por validar os meus comentários e modificações.              

        git checkout -b <nome da branch>:
        responsável por criar uma nova branch ou ramo.

        git checkout <nome da branch>:
        responsável por mudar de branch/ramo.

        git merge <nome_da_branch>:
        responsável por adicionar o conteúdo da branch atual no contéudo de outra branch.

        gitk:
        responsável por mostrar tudo que foi feito.

        git clone <url>:
        responsável por clonar/baixar todo o projeto do repositório remoto (link do repositório informado). 

        git push:
        responsável por subir as alterações para o repositório remoto (github)

        git pull:
        responsável por puxar as alteraões do repositório.

## Deu Erro? O que fazer
        
        Erro: 403
            Isto costuma acontecer muito caso o     
        terminal GIT já se encontre ativado por outro 
        usuário. É provavel que os usuários de GIT e 
        GITHUB sejam diferentes. Neste caso, acessar o 
        gerenciador de credenciais do windows e 
        remover o usuário que estiver ativo no git 
        resolerá o problema.

        Erro: Remote origin already exists
            Isso provavelmente está acontecendo porque você já tinha feito envio para este repositório.Para ter certeza, execute o comando "git remote" e deve aparecer "origin", indicando que o repositório remoto já tinha sido configurado no Github.
            Neste caso, partir direto pro comando "git push -u origin master" ao inves de usar o "git remote add origin" utilizado na primeira vez.

## Referência
    https://www.freecodecamp.org/portuguese/news/tutorial-de-git-e-github-controle-de-versao-para-iniciantes/
    
    https://readme.so/pt/editor

    https://cursos.alura.com.br/forum/topico-erro-remote-origin-already-exists-o-que-fazer-14236
