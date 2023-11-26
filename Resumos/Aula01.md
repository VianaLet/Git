# Comandos básicos do Git 📖🖊

## Tabela de Conteúdo
| Tópicos | Comando |
| ------  | ------- |
|[Iniciar um diretório no Git](#iniciar-um-diretório-no-git)| `git init` |
| [Criar novos documentos 📄](#criar-novos-documentos-📄)| `touch nome.extensão`
|[Criar pastas/diretórios 📂](#criar-pastasdiretórios-📂)| `mkdir nomepasta`|
|[Adicionar documentos criados e modificados no git](#adicionar-documentos-já-criados-e-modificados-no-git)| `git add nome` <br> `git add .` |
|[Visualizar os status do diretório](#visualizar-os-status-do-diretório)| `git status` |
|[Visualizar todos os commits realizados 🔎](#visualizar-todos-os-commits-realizados-🔎)| `git log`
|[Ignorar arquivos no .gitignore](#ignorar-arquivos-no-gitignore)| `echo nome/ > .gitignore`
| [Criar uma nova branch/ramo](#criar-uma-nova-branch) | `git checkout -b nomedabranch`
|[Mudar entre branches](#mudar-entre-branches)| `git checkout nomedabranch` |
|[Listar branchs do diretório](#listar-as-branchs-do-diretório) | `git branch`|

<br>

- ### Iniciar um diretório no Git:
     Este comando inicializa um repositório Git, criando a pasta oculta .git que armazena as configurações e histórico do projeto.

    ``` bash
    git init
    ```
    


<br>

- ### Criar novos documentos 📄
    Utilize este comando para criar novos arquivos no projeto, como o README.MD para documentação.

    ```
    touch nome.extensão
    # Exemplo: touch README.MD         touch Resumos/aula-01
    ```
<br>

- ### Criar pastas/diretórios 📂
    Crie novas pastas ou diretórios com este comando para organizar seu projeto de forma estruturada.

    ``` bash
    mkdir nomedapasta
        # Exemplo: mkdir Resumos       mkdir .gitinore
    ```
<br>

- ### Adicionar documentos já criados e modificados no git 
     Adicione documentos ao controle de versão do Git para prepará-los para o próximo commit.

    ``` bash
    git add nomedodocumento
     # Exemplo: git add README.MD
    ```
    ``` bash
    git add .  # adiciona todos os documentos modificados ou inseridos
     ```
    
<br>

- ### Visualizar os status do diretório 
    Este comando exibe o status das modificações no diretório, indicando arquivos não rastreados, modificados ou prontos para commit.

    ``` bash
    git status     
    ```
    Mostra as pastas que foram modificadas e não foram inseridas, ou se não teve nenhuma modificação no diretório

     <img src="../imagens/Cmd-Git status.PNG">
<br>

- ### Como visualizar todos os commits realizados 🔎 
    Visualize todos os commits feitos até o momento, incluindo informações sobre autor, data e mensagem de commit.
    ``` bash
    git log     
    ```    
    Mostra todos os commits feitos até o momento 
    
    <img src="../imagens/cmd-Git log.PNG">

<br>

- ### Ignorar arquivos no .gitignore 
    Utilize o .gitignore para especificar arquivos ou pastas a serem ignorados pelo Git, como arquivos temporários ou logs.

    ``` bash
    echo nomedapastaouarquivo/ > .gitignore
        
        # Exemplo: echo Resumos/ > .gitignore
    ```
<br>

- ### Criar uma nova branch
    Crie e mude para uma nova branch com este comando, útil para desenvolver recursos isoladamente.

    ``` bash
    git checkout -b nomedabranch
        # Exemplo: git checkout -b feature1
    ```
<br>

- ### Mudar entre branches
    Alterne entre branches existentes para trabalhar em diferentes partes do seu projeto.

    ```bash
    git checkout nomedabranch
    Exemplo:
    git checkout feature1
    ```
<br>

- ### Listar as branchs do diretório
    Este comando lista todas as branches no diretório, indicando a branch atual com um asterisco.

    ```bash
    git branch
    ```
    <img src="../imagens/cmd-Git branch.PNG">

