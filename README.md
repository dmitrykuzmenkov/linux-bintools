# kisstool
Utilites that help in everydays tasks in development.

## minify
Allows you to minify css and js files before you deploy it to production.
Usage: minify file.source.in > file.min.out

## watch-exec
Simple bash utility that helps you to run any command on any change in any folder
Usage: watch-exec folder command
You can use this as sync utility for special folder. For example using unison to sync folder on files change in it:
```bash
watch-exec source "unison -batch source ssh://remote/source"
```
That will run unison command if any file in folder source was changed.

## bash-colors
Display all colors to be used in your bash scripts
Usage: bash-colors

## git-branch-all
Show all branches on git repository with last commits and authors
Usage: git-branch-all
Show remotes: git-branch-all --remote

## git-branch-squash
Squash all commits in current branch since it was created using other branch
Usage: git-branch-squash [branch]
branch - branch that was used to create current branch to determine commits to squash. Default: master
