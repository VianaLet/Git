# Removendo e Desfazendo alterações no Repositório Local 🏠💻🗂
<br>

## Tabela de Conteúdo
| Tópicos | Comando |
| ------  | ------- |
| [Remover a pasta .git](#remover-a-pasta-git)| `git remove -rf .git`|
| [Restaurar/retornar ao último estado salvo do documento](#restaurar-retornar-ao-último-estado-salvo-do-documento)| `git restore nomearquivo"`|
|[Mudar o nome do último commit](#mudar-o-nome-do-último-commit)| `git commit --amend -m "novocomentário"`|
|[Pegar os arquivos do commit desejado e adicioná-los na área de preparação](#pegar-os-arquivos-do-commit-desejado-e-adicioná-los-na-área-de-preparação) | `git reset --soft númerodocommit`
|[Visualizar o histórico de commits mais detalhadamente](#visualizar-o-histórico-de-commits-mais-detalhadamente)| `git reflog`

- ### Remover a pasta .git
    ``` bash
    git remove -rf .git
    ```
    Este comando remove permanentemente o diretório .git, desfazendo completamente o controle de versão Git no repositório local.

<br>

- ### Restaurar/retornar ao último estado salvo do documento
    ``` bash
    git restore nomedoarquivo
    ```
    Utilize este comando para desfazer as alterações no arquivo e retornar ao último estado salvo, revertendo as modificações não commitadas.

<br>

- ### Mudar o nome do último commit
    <br>

    Se você precisa modificar a mensagem do último commit, utilize o seguinte comando:
    ```bash
    git commit --amend -m "novo comentário"
    git commit --amend -m "docs: atualizando Aula01.md e imagens"
    ```
    Este comando permite editar a mensagem do último commit, criando uma nova versão do commit com a mensagem ajustada.

    <img src="../imagens/cmd-Git commit --amend -m.PNG">

- ### Pegar os arquivos do commit desejado e adicioná-los na área de preparação
    ```bash
    git reset --soft númerodocommit
        # git reset --soft 7b351722d8c5f3f0ce06673385bc605ce3461bb5
    ```
    Utilize este comando para desfazer commits, mantendo as alterações na área de preparação. O "númerodocommit" é o identificador único do commit desejado.

- ### Visualizar o histórico de commits mais detalhadamente
    ``` bash
    git reflog
    ```
    Este comando exibe um log detalhado de todas as atividades do repositório, incluindo commits antigos e operações de desfazer.
    
    <img src="../imagens/cmd-Git reflog.PNG">