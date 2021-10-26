# GIT BASIC



### git init
```bash
$ cd ~
$ mkdir learn-git-local
$ cd learn-git-local
$ git init
$ ls -la
```
 
### clone existing repository
```bash
$ cd ..
$ git clone https://github.com/rezonjov/learn-git
$ code learn-git  # or open via VS Code manually
```
  
### git status & tracking files 
```bash
$ #on the same folder
$ cd workfolder
$ touch <NAME>.MD

$ # let's see the status after we create new file
$ git status 

$ # let's track the file
$ git add <NAME>.MD

$ # let's check status
$ git status

$ # let's change file
$ vim <NAME>.MD

$ # let's see the status again
$ git status
```
 
### clear & reset

```bash 
$ git reset 
 
```
 