# HDC-Git e GitHub, do básico ao avançado.

ÍNDICE 

1. Introdução;
2. Git fundamental;
3. Trabalhando com Branches;
4. Compartilhamento e atualização de repositórios;
5. Análise e inspeção de repositórios;
6. Administração de repositórios;
7. Explorando o GitHub;
8. Markdown;
9. Projeto com GitHub Pages;
10. Encerramento e próximos passos;
___________________________________________________

## 1 - INTRODUÇÃO.

* Instalando o git no Linux:
    No GNU\Linux, basta executar no terminal o comando:
        sudo apt install git
    Para distribuições baseadas no Debian com empacotamento apt, o pacote já está nos repositórios por padrão.
    
* Instalando o Visual Studio Code ( IDE ):
    No GNU\Linux, basta executar no terminal o comando:
        sudo apt install code
    Para distribuições baseadas no Debian com empacotamento apt, o pacote já está nos repositórios por padrão.
    
* O que é controle de versão?
    Uma técnica que ajuda a gerenciar o código-fonte de uma aplicação, registrando todas as modificações de código, podendo também reverte- las. Criar versões de um software em diferentes estágios, podendo alterar facilmente entre elas. Cada membro da equipe pode trabalhar em uma versão diferente. No caso aqui, aprenderemos a usar o GIT, uma ferramenta de controle de versão.
    
* O que é GIT ?
    O sistema de controle de versão mais utilizado no mundo atualmente, é baseado em repositórios que contém todas as versões do código e também as cópias de cada desenvolvedor. Todas as operações do GIT são otimizadas para terem alto desempenho e os objetos são protegidos com criptografia para evitar alterações indevidas e maliciosas. o GIT é uma ferramenta do mundo open source, ou seja é de código aberto.

# 2 - GIT FUNDAMENTAL.

* Primeiramente, um repositório é um local onde um código esta armazenado, na maioria das vezes cada projeto tem seu repositório. Quando criamos um repositório estamos iniciando um novo projeto e este repositório pode ser enviado para um servidor especializado em gerenciar repositórios, como o GitHub.
    Cada pessoa que tiver acesso a certo repositório, poderá baixar e criar versões diferentes de um mesmo projeto em sua máquina.
    
* Criando o primeiro repo:
    Para criarmos um repositório utilizamos o comando:
        git init
    Desta maneira o git vai criar os arquivos necessários para inicializa- lo em uma pasta oculta chamada de ".git".
    Após este comando o diretório atual será reconhecido como um projeto pelo git e responderá aos seus demais comandos.
    
* O que é o GitHub ?
    É um serviço para gerenciar repositórios, gratuito e amplamente utilizado. Podemos enviar nossos projetos para o GH e disponibiliza- lo para outros desenvolvedores. O GH é gratuito para projeto públicos e privados.
    Crie sua conta em https://www.github.com
    
* Enviando repositórios para o GH.
    Podemos facilmente enviar nossos repos para o GH.
    Precisamos criar o projeto no GitHub, inicializar o mesmo no git em nossa máquina, sincronizar com o GH e enviar, esta sequência que parece complexa, é facilmente executada com poucos comandos, isso é feito uma vez por projeto. Alguns dos comandos a seguir serão novamente utilizados durante o curso.
    git init - Inicia o repositório git local;
    git add <file> ou . - Adiciona o arquivo ou todo o diretório ao repo;
    git commit -m "commit name" - Nomeia o commit, pode- se dizer a versão.
    git push - empurra o repositório para o GitHub, depois de configura- lo. Essa parte de configuração é feita durante a criação do repositório no GitHub.
    
* Verificando mudanças no projeto.
    As mudanças do projeto podem ser verificadas pelo comando:
        git status
    Este comando é utilizado muito frequentemente, usado para mapear todas as alterações do projeto, como arquivos não monitorados e arquivos modificados. Pode- se dizer também que é a diferença do que já foi enviado ao servidor ou salvo no projeto.

* Adicionando arquivos ao projeto.
    Para adicionar arquivos a um projeto utilizados o comando:
        git add
    Podemos adicionar um arquivo específico como também diversos de uma só vez. Somando adicionando arquivos eles serão monitorados pelo git, ou seja, se não adicionar ele não estará no controle de versão.
    É interessante utilizar este comando de tempos em tempos para não perder algop por descuido.

* Salvando alterações no projeto.
    As alterações salvas do projeto são realizadas pelo comando:
        git commit
    Podemos commitar arquivos específicos ou vários de uma vez com a flag -a. É uma boa prática nomear com uma mensagem cada novo commit. Usamos a flag -m para adicionar a mensagem.
        git commit -m "Msg aqui"

* Enviando código ao repositório remoto.
    Quando finalizamos uma funcionalidade nova, enviamos ao repo remoto, o código fonte, esta ação é feita através do comando:
        git push
    Após esta ação o código do servidor será atualizado baseando- se no código local enviado;

* Recebendo as mudanças
    É comum também ter que sincronizar o local com as mudanças do remoto, esta ação é feita pelo comando:
        git pull
    Após o comando serão buscadas atualizações, se encontradas elas serão unidas no código atual em nossa máquina.

* Clonando repositórios.
    O ato de baixar um repo de um servidor remoto é chamado de clonar o repositório.
    Para realizar esta ação, usamos o comando:
        git clone
    Passando a referência do repositório remoto, este comando é utilizado quando entramos em um novo projeto, por exemplo.

* Removendo arquivos do repositório.
    Os arquivos podem ser deletados da monitoração do git usando o comando:
        git rm
    Após deletar um arquivo do git ele não terá mais suas atualizações consideradas pelo git, apenas quando for adicionado pelo git add.

* Verificando alterações por meio de logs.
    Podemos acessar um log de modificações feitas no projeto, para isso usamos o comando:
        git log
    Você receberá uma informação dos commits realizados no projeto até então.

* Renomeando arquivos.
    Podemos renomear arquivos em nosso repositório usando o seguinte comando:
        gir mv <file>
    O mesmo também pode ser movido para putra pasta e isso fará com que este novo arquivo seja monitorado pelo git. 
O arquivo anterior é excluído.

* Desfazendo alterações.
    O arquivo modificado pode ser retornado ao estado original com o comando:
        git checkout
    Após a utilização do mesmo o arquivo sai do staging, caso seja feita uma próxima alteração, ele entra em staging novamente.