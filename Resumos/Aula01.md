# Comandos básicos do Git 📖🖊

## Tabela de Conteúdo
| Tópicos | Comando |
| ------  | :-------: |
|[Iniciar um diretório no Git](#iniciar-um-diretório-no-git)| `git init` |
| [Criar novos documentos 📄](#criar-novos-documentos-📄)| `touch nome.extensão`
|[Criar pastas/diretórios 📂](#criar-pastasdiretórios-📂)| `mkdir nomepasta`|
|[Adicionar documentos criados e modificados no git](#adicionar-documentos-já-criados-e-modificados-no-git)| `git add nome` <br> `git add .` |
|[Visualizar os status do diretório](#visualizar-os-status-do-diretório)| `git status` |
|[Visualizar todos os commits realizados 🔎](#visualizar-todos-os-commits-realizados-🔎)| `git log`
|[Ignorar arquivos no .gitignore](#ignorar-arquivos-no-gitignore)| `echo nome/ > .gitignore`
| [Criar uma nova branch/ramo](#criar-uma-nova-branch) | `git checkout -b nomedabranch`
|[Remover uma branch](#remover-uma-branch)|`git -d nomedabranch`|
|[Mudar entre branches](#mudar-entre-branches)| `git checkout nomedabranch` |
|[Visualizar o último commit de cada branch](#visualizar-o-último-commit-de-cada-branch)| `git branch -v`
|[Listar branchs do diretório](#listar-as-branchs-do-diretório) | `git branch`|
|[Mesclar branches](#mesclar-branches)|`git merge nome da branch`|

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

### Remover uma branch
Remova uma branch que já foi completamente mesclada com a branch principal (geralmente "master").

    ```bash
    git branch -d nomedabranch
    ```
    Substitua "nomedabranch" pelo nome da branch que deseja excluir.

<br>


- ### Mudar entre branches
    Alterne entre branches existentes para trabalhar em diferentes partes do seu projeto.

    ```bash
    git checkout nomedabranch
    Exemplo:
    git checkout feature1
    ```
<br>

### Visualizar o último commit de cada branch
Visualize o último commit de cada branch no diretório.

    ```bash
    git branch -v
    ```
Isso fornecerá informações sobre o último commit em cada branch, incluindo o hash do commit, a mensagem e a data.

<br>

- ### Listar as branchs do diretório
    Este comando lista todas as branches no diretório, indicando a branch atual com um asterisco.

    ```bash
    git branch
    ```

    <img src="../imagens/cmd-Git branch.PNG">

<br>


### Mesclar branches
Mesclar alterações de uma branch para outra, por exemplo, para incorporar as alterações de uma feature branch de volta para a branch principal.

    ```bash
    git merge nome-da-branch
    ```

Substitua "nome-da-branch" pelo nome da branch que você deseja mesclar com a branch atual.