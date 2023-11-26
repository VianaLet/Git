# Comandos básicos do Git 📖🖊

## Tabela de Conteúdo
| Tópicos | Comando |
| ------  | ------- |
|[Para iniciar um diretório no Git](#para-iniciar-um-diretório-no-git)| `git init` |
| [Para criar novos documentos 📄](#para-criar-novos-documentos-📄)| `touch nome.extensão`
|[Para criar pastas/diretórios 📂](#para-criar-pastasdiretórios-📂)| `mkdir nomepasta`|
|[Adicionar documentos criados e modificados no git](#adicionar-documentos-já-criados-e-modificados-no-git)| `git add nome` <br> `git add .` |
|[Como visualizar os status do diretório](#como-visualizar-os-status-do-diretório)| `git status` |
|[Como visualizar todos os commits realizados 🔎](#como-visualizar-todos-os-commits-realizados-🔎)| `git log`
|[Colocar um arquivo dentro do .gitignore](#colocar-um-arquivo-dentro-do-gitignore)| `echo nome/ > .gitignore`
| [Criar uma nova branch/ramo](#criar-uma-nova-branch) | `git checkout -b nomedabranch`
|[Mudar entre branches](#mudar-entre-branches)| `git checkout nomedabranch` |
|[Saber quais são as branchs do diretório](#saber-quais-são-as-branchs-do-diretório) | `git branch`|

<br>

- ### Para iniciar um diretório no Git:
    ``` bash
    git init
    ```
    Com esse comando o git vai criar uma pasta oculta chamada .git

<br>

- ### Para criar novos documentos 📄
    ```
    touch nome.extensão
    Exemplos:
    touch README.MD         touch Resumos/aula-01
    ```
<br>

- ### Para criar pastas/diretórios 📂
    ```
    mkdir nomedapasta
        Exemplos:
        mkdir Resumos       mkdir .gitinore
    ```
<br>

- ### Adicionar documentos já criados e modificados no git 
    ``` bash
    git add nomedodocumento
    Exemplo:
    git add README.MD
    ```
    ```
    git add .  //adicionar todos os documentos que foram inseridos ou modificados
     ```
    
<br>

- ### Como visualizar os status do diretório 
    ``` bash
    git status     
    ```
    Mostra as pastas que foram modificadas e não foram inseridas, ou se não teve nenhuma modificação no diretório

     <img src="../imagens/Cmd-Git status.PNG">
<br>

- ### Como visualizar todos os commits realizados 🔎 
    ``` bash
    git log     
    ```    
    Mostra todos os commits feitos até o momento 
    
    <img src="../imagens/cmd-Git log.PNG">

<br>

- ### Colocar um arquivo dentro do .gitignore 
    ``` bash
    echo nomedapastaouarquivo/ > .gitignore
        Exemplo:
        echo Resumos/ > .gitignore
    ```
<br>

- ### Criar uma nova branch
    ``` bash
    git checkout -b nomedabranch
    Exemplo:
    git checkout -b feature1
    ```
<br>

- ### Mudar entre branches
    ```bash
    git checkout nomedabranch
    Exemplo:
    git checkout feature1
    ```
<br>

- ### Saber quais são as branchs do diretório
    ```bash
    git branch
    ```
    <img src="../imagens/cmd-Git branch.PNG">