# git-academy-22

## Inicialização de um projeto:
```
git init
```

## Configurações iniciais
```bash
git config --global user.name "username"
git config --global user.email "user@email.com"
```

## Controle de alterações
Para visualizar as alterações feitas, vamos usar:
```bash
git status
```

## Criando commits
Primeiramente precisamos adicionar as mudanças:
> utilize o ponto (.) para adicionar todas as alterações do projeto.
```bash
git add .
```
E enfim 'commitar' usando:
```bash
git commit -m "descricao das alteracoes"
```

## Branches
- Podemos ramificar o código usando branches para criar uma nova, executamos:
```bash
git switch --create <nome-da-nova-branch>
# ou
git checkout -b <nome-da-nova-branch>
```
- Listando branches criadas:
```bash
git branch
```
Apagando branches:
```bash
git branch -D <nome-da-branch>
```

## Github
- Adicionando um remote origin:
```bash
git remote add origin <link do .git no github>

# exemplo
git remote add origin https://github.com/user/repo-name.git
```
- Subindo alterações:
```bash
git push origin <nome-da-branch>

# caso a branch nao exista no Github, use:
git push -u origin <nome-da-branch> # ele criara a nova branch no Github
```