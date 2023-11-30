# Enviando e Baixando Alterações com o Repositório Remoto 📤🖥🌐

## Tabela de Conteúdo
| Tópicos | Comando |
| ------  | ------- |
| [Linkar um repositório local com o remoto](#linkar-um-repositório-local-com-o-remoto)| `git remote add origin URL do repositório`|
| [Enviar alterações do repositório local para o remoto](#enviar-alterações-do-repositório-local-para-o-remoto)| `git push origin nomebranch`|
| [Baixar alterações do repositório remoto para o local](#baixar-alterações-do-repositório-remoto-para-o-local)| `git pull`|
| [Baixar as alterações do repositório remoto sem realizar a merge](#baixar-as-alterações-do-repositório-remoto-sem-realizar-a-merge)| `git fetch`|
| [Clonar somente uma branch de um repositório remoto](#clonar-somente-uma-branch-de-um-repositório-remoto)| `git clone URLdorepositório --branch teste --single-branch`|
| [Arquivar as alterações](#arquivar-as-alterações)|`git stash`|
| [Visualizar quais são as alterações arquivadas](#visualizar-quais-são-as-alterações-arquivadas)|`git stash list`|
| [Trazer as alterações arquivadas e escolher a alteração mais recente](#trazer-as-alterações-arquivadas-e-escolher-a-alteração-mais-recente)|`git stash pop`|
| [Trazer as alterações arquivadas e manter as alterações feitas anteriormente](#trazer-as-alterações-arquivadas-e-manter-as-alterações-feitas-anteriormente)| `git stash apply`|

---

- ### Linkar um repositório local com o remoto
    Este comando estabelece uma conexão entre um repositório local e um repositório remoto. Substitua "URL do repositório" pela URL do seu repositório remoto.

    ```bash
    git remote add origin URL-do-Repositório
    ```
    Isso cria um link chamado "origin" para o repositório remoto.

---

- ### Enviar alterações do repositório local para o remoto
    Envie as alterações locais para o repositório remoto. Substitua "nomebranch" pelo nome da branch que você deseja enviar.

    ```bash
    git push origin nomebranch
    ```
    Isso atualiza o repositório remoto com as alterações feitas localmente.

---

- ### Baixar alterações do repositório remoto para o local
    Atualize o repositório local com as alterações do repositório remoto. Isso combina `git fetch` e `git merge`.

    ```bash
    git pull
    ```
    Isso baixa e mescla automaticamente as alterações do repositório remoto para o seu repositório local.

---

- ### Baixar as alterações do repositório remoto sem realizar a merge
    Baixe as alterações do repositório remoto sem mesclá-las automaticamente. Este comando é útil para revisar as alterações antes de incorporá-las.

    ```bash
    git fetch
    ```
    Isso baixa as alterações do repositório remoto, mas não as mescla automaticamente no seu repositório local.

---

- ### Clonar somente uma branch de um repositório remoto
    Clone apenas uma branch específica de um repositório remoto. Substitua "URLdorepositório" pela URL do repositório e "teste" pelo nome da branch.

    ```bash
    git clone URL-do-Repositório --branch teste --single-branch
    ```
    Isso cria uma cópia local apenas da branch especificada.

---

- ### Arquivar as alterações
    Guarde temporariamente as alterações não commitadas para aplicar em outro momento.

    ```bash
    git stash
    ```
    Isso arquiva as alterações para que você possa alternar para outra branch ou aplicar posteriormente.

---

- ### Visualizar quais são as alterações arquivadas
    Exiba uma lista de todas as alterações arquivadas.

    ```bash
    git stash list
    ```
    Isso mostra todas as alterações arquivadas, identificadas por um índice.

---

- ### Trazer as alterações arquivadas e escolher a alteração mais recente
    Reaplique as alterações arquivadas ao seu branch de trabalho e remova a alteração mais recente do stash.

    ```bash
    git stash pop
    ```
    Isso aplica a alteração mais recente do stash e a remove da lista de alterações arquivadas.

---

- ### Trazer as alterações arquivadas e manter as alterações feitas anteriormente
    Reaplique as alterações arquivadas ao seu branch de trabalho, mantendo a lista de alterações arquivadas.

    ```bash
    git stash apply
    ```
    Isso aplica a alteração mais recente do stash, mas mantém a alteração na lista de alterações arquivadas.

---

Lembre-se de ajustar as URLs e os nomes de branches conforme necessário para o seu contexto. Este README oferece uma visão geral dos comandos para enviar e baixar alterações com o repositório remoto.