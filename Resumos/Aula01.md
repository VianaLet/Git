# Comandos básicos do Git 📖🖊

## Tabela de Conteúdo
| Tópicos | Comando |
| ------  | ------- |
|[Para iniciar um diretório no Git](#para-iniciar-um-diretório-no-git)| git init |
| [Para criar novos documentos 📄](#para-criar-novos-documentos-📄)| touch nome.extensão
|[Para criar pastas/diretórios 📂](#para-criar-pastasdiretórios-📂)| mkdir nomepasta|
|[Adicionar documentos criados e modificados no git](#adicionar-documentos-já-criados-e-modificados-no-git)| git add nome <br> git add . |
|[Como visualizar os status do diretório](#como-visualizar-os-status-do-diretório)| git status |
|[Como visualizar todos os commits realizados 🔎](#como-visualizar-todos-os-commits-realizados-🔎)| git log
|[Colocar um arquivo dentro do .gitignore](#colocar-um-arquivo-dentro-do-gitignore)| echo nome/ > .gitignore
- ### Para iniciar um diretório no Git:
    ``` bash
    git init
    ```
    Com esse comando o git vai criar uma pasta oculta chamada .git

- ### Para criar novos documentos 📄
    ```
    touch nome.extensão
    Exemplos:
    touch README.MD         touch Resumos/aula-01
    ```
- ### Para criar pastas/diretórios 📂
    ```
    mkdir nomedapasta
        Exemplos:
        mkdir Resumos       mkdir .gitinore
    ```
- ### Adicionar documentos já criados e modificados no git 
    ```
    git add nomedodocumento
    Exemplo:
    git add README.MD
    git add . (esse aqui vamos adicionar todos os documentos que foram inseridos ou modificados)
    ```

- ### Como visualizar os status do diretório
    ```
    git status      (vai mostrar as pastas que foram modificadas e não foram inseridas, ou se não teve nenhuma modificação no diretório)
    ```
     <img src="../imagens/cmd-Git status.PNG">
- ### Como visualizar todos os commits realizados 🔎 
    ``` 
    git log     Mostra todos os commits feitos até o momento
    ```     
    <img src="../imagens/cmd-Git log.PNG">
    

- ### Colocar um arquivo dentro do .gitignore 
    ```
    echo nomedapastaouarquivo/ > .gitignore
        Exemplo:
        echo Resumos/ > .gitignore
    ```
