# kisstool

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
