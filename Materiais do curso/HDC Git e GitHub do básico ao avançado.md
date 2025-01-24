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

    Primeiramente, um repositório é um local onde um código esta armazenado, na maioria das vezes cada projeto tem seu repositório. Quando criamos um repositório estamos iniciando um novo projeto e este repositório pode ser enviado para um servidor especializado em gerenciar repositórios, como o GitHub.
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

* 
