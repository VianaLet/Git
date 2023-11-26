# Configurações Iniciais do Git 📖🖊

## Tabela de Conteúdo

| Tópicos | Comando |
| ------  | ------- |
| [Configurar nome e email Global](#configurar-nome-e-email)| `git config --global user.name "Seu Nome"` <br> `git config --global user.email "seuemail@example.com"`|
| [Configurar nome e email local](#configurar-nome-e-email-local)| `git config user.name "Seu Nome"` <br> `git config user.email "seuemail@example.com"`|
| [Clonar um repositório existente](#clonar-um-repositório-existente)| `git clone URL-do-Repositório`|

---

- ### Configurar nome e email
    Antes de começar a usar o Git, é importante configurar seu nome e endereço de e-mail. Estas informações são associadas aos seus commits. Utilize os seguintes comandos no terminal, substituindo "Seu Nome" e "seuemail@example.com" pelos seus dados:

    ```bash
    git config --global user.name "Seu Nome"
    git config --global user.email "seuemail@example.com"
    ```
    Essas configurações são globais e serão aplicadas a todos os seus repositórios Git no sistema.
- ### Configurar nome e email local
    Se você deseja configurar um nome e endereço de e-mail específicos para um projeto específico, use os seguintes comandos dentro do diretório do projeto:

    ```bash
    git config user.name "Seu Nome"
    git config user.email "seuemail@example.com"
    ```
    Essas configurações locais substituirão as configurações globais apenas para o repositório atual.

    
- ### Clonar um repositório existente
    Para começar a trabalhar com um repositório existente, clone-o para o seu ambiente local. Utilize o comando abaixo, substituindo "URL-do-Repositório" pela URL do repositório que você deseja clonar:

    ```bash
    git clone URL-do-Repositório
    ```
    Isso criará uma cópia do repositório na sua máquina local, permitindo que você contribua ou trabalhe nos arquivos do projeto.