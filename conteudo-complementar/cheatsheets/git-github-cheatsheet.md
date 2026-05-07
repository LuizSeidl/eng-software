# 📋 Git & GitHub Cheatsheet

## Configuração inicial
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@email.com"

## Repositório
git init              # inicia repositório local
git clone <url>       # clona repositório remoto

## Status e histórico
git status            # mostra arquivos modificados
git log               # histórico de commits
git log --oneline     # histórico resumido

## Adicionar e commitar
git add .             # adiciona tudo
git add <arquivo>     # adiciona arquivo específico
git commit -m "msg"   # cria commit

## Branches
git branch                # lista branches
git branch <nome>         # cria branch
git branch -m <novo-nome> # renomeia a branch atual
git checkout <nome>       # muda de branch
git checkout -b <nome>    # cria e muda de branch
git merge <nome>          # merge de branch

## Rebase
git rebase main        # reaplica commits da branch atual em cima da main
git rebase --abort     # cancela o rebase em caso de conflito
git rebase --continue  # continua o rebase após resolver conflito

## Merge vs Rebase
# merge  — preserva histórico, gera commit de merge
# rebase — histórico linear, reescreve commits
# dica: use rebase em branches locais, merge em branches compartilhadas

## Remoto
git remote add origin <url>  # conecta repositório remoto
git push -u origin main      # primeiro push
git push                     # push normal
git pull                     # atualiza local

## Desfazer
git restore <arquivo> # descarta alterações
git reset HEAD~1      # desfaz último commit

## Diferenças e Arquivos Ignorados
git diff              # mostra alterações não adicionadas (staged)
git diff --staged     # mostra alterações prontas para commit
.gitignore            # arquivo onde se lista o que o git deve ignorar

## Stash (Área de rascunho)
git stash             # guarda alterações não commitadas temporariamente
git stash pop         # recupera as alterações guardadas
