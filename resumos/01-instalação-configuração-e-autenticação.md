
# DIO | Versionamento de código com Git e GitHub

## Intalação, Connfiguração e Autenticação

### Instalando git no Windows
- Acesse <https://git-scm.com/downloads>    
- Faça o download do instalador e execute
- Aceite a licença, clique em "Next" e contiue configurando de acordo com a sua preferência
- Finalize clicando em "Install" e "Finish"

## 

### Instalando o Git no Linux (Ubuntu)
- Confira a doc.: < https://git-scm.com/download/linux >;
- Instale a última versão estável do Git:

    ```bash
    # add-apt-repository ppa:git-core/ppa
    ```
    ```bash
    # apt update
    ```
    ```bash
    # apt install git
    ```
## 

### Instalando o Git no macOS
- Confira a doc.: < https://git-scm.com/download/mac >;
- Instale o Homebrew: < https://brew.sh/ >;
- Instale o Git:
    ```
    $ brew install git
    ```
## 

### Configurando o Git

Listando configurações do git:

```bash
$ git config --global --list
```

Configurando com seu nome de usuário e email (globalmente):
    
```bash
$ git config --global user.name "Nome"
```
```bash
$ git config --global user.email seuemail@email.com
```

Configurando o nome da branch padrão:
    
```bash
$ git config --global init.defaultBranch main
```
## 

### Autenticando via Token

- Para gerar um novo token, acesse: https://github.com/settings/tokens/new 
- Copie o token e salve em um local seguro;
- Clone o repositório remoto com a URL HTTPS:

    ```bash
    $ git clone URL
    ```
- Selecione a opção token;
- Cole o token e realize a autenticação;
- Defina uma credencial:

    ```bash
    $ git config --global credential.helper store
    ```
    ou
    ```bash
    $ git config --global credential.helper cache
    ```
## 

### Autenticando via chave SSH

- [Verifique se há chaves SSH](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/checking-for-existing-ssh-keys?platform=windows#checking-for-existing-ssh-keys);
- [Gere uma nova chave SSH](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key);
- [Adicione sua chave SSH ao ssh-agent](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#adding-your-ssh-key-to-the-ssh-agent)
- [Adicione sua chave SSH ao GitHub](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account#adding-a-new-ssh-key-to-your-account);

##

