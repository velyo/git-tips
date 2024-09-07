## Git Aliases

This is a collection of some usefule git aliases.

git status shortcut [usage: git st]
```
git config --global alias.st status
```

checkout shortcut [usage: git co dev]
```
git config --global alias.co checkout
```

create branch shortcut [usage: git br BRANCH]
```
git config --global alias.br branch
```

create a new branch and switch to it [usage: git cb BB-0000]
```
git config --global alias.cb “checkout -b”
```

add and commit all changes with comment [usage: git ci “BB-0000 issue”]
```
git config --global alias.ci '!git add -A && git commit -m'
```

add changes to last commit [usage: git append]
```
git config --global alias.append "!git add -A ; git commit --amend --no-edit -C HEAD"
```

push a new local branch to the upstream [usage: git put BB-0000]
```
git config --global alias.put “push --set-upstream origin”
```

stop tracking a file [usage: git forget test.txt]
```
git config --global alias.forget "update-index --assume-unchanged"
```

rollback the last commit [usage: git rollback]
```
git config --global alias.rollback “reset --soft HEAD~”
```

decorated log [usage: git lga]
```
git config --global alias.lga "log --graph --oneline --all --decorate"
```

uncommit the last commit [usage: git uncommit]
```
git config --global alias.uncommit “reset HEAD~”
```

unstage the added changes [usage: git unstage]
```
git config --global alias.unstage 'reset HEAD --'
```

```
git config --global alias.hist 'log --pretty=format:"%h %ad | %s%d [%an]" --graph --date=short'
git config --global alias.type 'cat-file -t'
git config --global alias.dump 'cat-file -p'
git config --global alias.last 'log -1 HEAD'
```