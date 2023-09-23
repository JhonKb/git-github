
# DIO | Versionamento de código com Git e GitHub

## Criando e Clonando Repositórios

Iniciando repositório git:
```bash
$ git init
```

Clonando repositório:
```bash
$ git clone URL novo-nome(opcional)
```

Verificando se o repositório já está conectado:
```bash
$ git remote -v
```

Conectando repositório local com o remoto:
```bash
$ git remote add origin URL
```
##


## Salvando Alterações no Repositório

- Avóre de Trabalho - Local onde ficam as alterções recentes;
- Área de Preparação - Local onde as alterações são salvas antes de serem commitadas;

Verificando status:
```bash
$ git status
```

Adicionando à área de preparação:
- Todos as alterações
    ```bash
    $ git add .
    ```
- Alteração específica
    ```bash
    $ git add exemplo.arquivo
    ```

Commitando:
```bash
$ git commit -m"mensagem do commit"
```

Exibindo o histórico de commits:
```bash
$ git log
```
##

## Desfazendo Alterações no Repositório Local

Restaurando arquivo modificado:
```bash
$ git restore exemplo.arquivo
```

Alterando mensagemdo ultimo commit:
```bash
$ git commit --amend -m"nova mensagem"
```

Retornando no "tempo" para um commit:

- Retorna as alterações posteriores para a área de preparação
    ```bash
    $ git reset --soft código-commit
    ```
- Retorna as alterações para a árvore de trabalho 
    ```bash
    $ git commit --mixed código-commit
    ```
- Apaga completamente as alterações
    ```bash
    $ git commit --hard código commit
    ```

Exibindo histórico detalhado das alterações:
```bash
$ git reflog
```

Removendo arquivo da área de preparação:
```bash
$ git reset exemplo.arquivo
```
ou
```bash
$ git restore --staged exemplo.arquivo
```
##

## Enviando e Baixando Alterações Com o Repositório Remoto

Enviando alterações para o repositório remoto:
```bash
$ git push -u origin main
```

Baixando alterações do repositório remoto:
```bash
$ git pull
```
##

## Trabalhando com Branchs 

Listando branchs:
```bash
$ git branch 
```
ou
```bash
$ git branch -v
```

Criando nova branch:
```bash
$ git branch checkout -b nome-branch
```

Trocando de branch:
```bash
$ git branch checkout nome-branch
```

Mesclando branchs:
```bash
$ git merge nome-branch
```

Excluindo branch:
```bash
$ git branch -d nome-branch
```
##

## Trabalhando com Branchs - Comandos Úteis no Dia a Dia

Baixando alterações do repositório remoto sem mesclar:
```bash
$ git fetch origin main
```

Exibindo diferença entre branch remota e local:
```bash
$ git diff main origin/main
```

Mesclando com o repositório local:
```bash
$ git merge origin/main
```

Clonando branch específica:
```bash
$ git clone URL --branch nome-branch --sigle-branch
```

Arquivando modificação:
```bash
$ git stash
```

Listando arquivo de modificação:
```bash
$ git stash list
```

Desfazendo alteração e apagando do arquivo de modificação:
```bash
$ git stash pop
```

Desfazendo alteração e mantendo no arquivo de modificação:
```bash
$ git stash apply
```
##