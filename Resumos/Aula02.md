# Removendo e Desfazendo alterações no Repositório Local 🏠💻🗂
<br>

## Tabela de Conteúdo
| Tópicos | Comando |
| ------  | ------- |
| [Como remover a pasta .git](#como-remover-a-pasta-git)| `git remove -rf .git`|
| [Como restaurar/ retornar ao último estado salvo do documento](#como-restaurar-retornar-ao-último-estado-salvo-do-documento)| `git retore nomearquivo"`|
|[Como mudar o nome do último commit](#como-mudar-o-nome-do-último-commit)| `git commit --amend -m "novocomentário"`|
|[Pegar os arquivos que estão no commit que queremos e adicionarmos na área de preparação](#pegar-os-arquivos-que-estão-no-commit-que-queremos-e-adicionarmos-na-área-de-preparação) | `git reset --soft númerodocommit`
|[Visualizar o histórico de commits mais detalhadamente](#visualizar-o-histórico-de-commits-mais-detalhadamente)| `git reflog`

- ### Como remover a pasta .git
    ``` bash
    git remove -rf .git
    ```
<br>

- ### Como restaurar/ retornar ao último estado salvo do documento
    Bom tomar certo cuidado, pois se tiverem alterações na área de staged atual que você queira permanecer, você irá perder pois o git vai retornar a versão anterior dessa, no caso o commit anterior
    ``` bash
    git restore nomedoarquivo
    ```
<br>

- ### Como mudar o nome do último commit
    <br>

    Temos o último commit como "docs: upadate Aula01.md and images:

    <img src="../imagens/ultimo commit.PNG">

    Mas queremos mudar o que está escrito nesse commit então colocamos o seguinte código no terminal
    ```bash
    git commit --amend -m "novo comentário"
    git commit --amend -m "docs: atualizando Aula01.md e imagens"
    ```
    Vamos ver como fica:
    <img src="../imagens/cmd-Git commit --amend -m.PNG">

- ### Pegar os arquivos que estão no commit que queremos e adicionarmos na área de preparação
    Nessa ocasião estamos pegando o número aleatorio que o git cria para informar que queremos resetar o commit. Como tem o --soft ele vai tirar todas as pastas do commit e adicionar a nossa área de trabalho atual
    ```bash
    git reset --soft chavedocommit
    ```
- ### Visualizar o histórico de commits mais detalhadamente
    ``` bash
    git reflog
    ```
    <img src="../imagens/cmd-Git reflog.PNG">