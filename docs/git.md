### clonar repositório

```
git clone git@github.com:user/repositorio.git
```

### definir usuário somente em um diretório

```
git config user.email "user@gmail.com"
git config user.name "User"
```

### definir usuário global

```
git config --global user.email "user@gmail.com"
git config --global user.name "User"
```

### atualizar repositório local (remote >> local) 

```
git pull
```

### se não for fazer commit (branch diferente da main), mas quiser fazer pull

```
git stash
```

### criar branch

```
git checkout -b name_branch

```
### deletar branch 
```
git branch -D nome_branch

```
### trocar de branch
```
git checkout name_branch

```
### inicializar novo repositório por linha de comando

```
echo "# test" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:user/repositorio.git
git push -u origin main
```

### inicializar repositório existente por linha de comando

```
git remote add origin git@github.com:lorranavf/test.git
git branch -M main
git push -u origin main
```

### atualizar repositório (local >> remote)

```
git add . 
git commit -m ':type: message'
git push origin name_branch
```

### definir pull a partir do main se você estiver em uma branch diferente da main

```
git branch --set-upstream-to=origin/main name_branch
```
### ou
```
git checkout main
git pull
git checkout branch_de_trabalho
git merge main
```

### rotina de trabalho no repositório (criando branchs)

```
git checkout main
git pull
git checkout -b name_new_branch
git add .
git commit -m 'message'
git push origin name_new_branch
git checkout main
git branch -D name_new_branch

```

### outra possibilidade (trabalhar sempre com a mesma branch de trabalho)

```
git checkout main
git pull
git checkout name_branch_de_trabalho
git merge main
git add .
git commit -m 'message'
git push origin name_branch_de_trabalho
```

# Importante

1. Crie branchs de desenvolvimento para validar novas funcionalidades.
2. Escreva commits significativos. [Padrões de commit](https://github.com/iuricode/padroes-de-commits).



