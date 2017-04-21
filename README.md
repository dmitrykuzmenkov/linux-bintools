# linux-bintools
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
**branch** - branch that was used to create current branch to determine commits to squash. Default: master  

## git-tag-date
Show all tags for current branch with its creation date  
Usage: git-tag-date  

## git-stat-summary
Show summary statistic of lines changes for special author since custom date  
Usage: git-stat-summary --author=[git-name] --since=[since-date] --until=[until-date]  
**git-name** - Git commit author name or email  
**since-date** - Date to start searching for stat (git --since format) (optional)  
**until-date** - Date to end (git --until format) (optional)  

## git-commit-recent
Show recent commit and branches where that commits were done  
Usage: git-commit-recent  

## swap-usage
Show top proccesses and amount of swap they use.  
Usage: swap-usage

## psql-table-recreate
Recreate existing table using other schema to optimize indexes usage
Usage: psql-table-recreate --db=database --table=table

## shuffle
Shuffle lines using pipe  
Usage: cat file | shuffle

## generate-htpasswd
Generate .htpasswd file for HTTP Auth  
Usage: generate-htpasswd [user] [password]  
**user** - username  
**password** - raw password you want
