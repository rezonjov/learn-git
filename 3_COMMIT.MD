     ██████╗ ██╗████████╗     ██████╗ ██████╗ ███╗   ███╗███╗   ███╗██╗████████╗
    ██╔════╝ ██║╚══██╔══╝    ██╔════╝██╔═══██╗████╗ ████║████╗ ████║██║╚══██╔══╝
    ██║  ███╗██║   ██║       ██║     ██║   ██║██╔████╔██║██╔████╔██║██║   ██║   
    ██║   ██║██║   ██║       ██║     ██║   ██║██║╚██╔╝██║██║╚██╔╝██║██║   ██║   
    ╚██████╔╝██║   ██║       ╚██████╗╚██████╔╝██║ ╚═╝ ██║██║ ╚═╝ ██║██║   ██║   
     ╚═════╝ ╚═╝   ╚═╝        ╚═════╝ ╚═════╝ ╚═╝     ╚═╝╚═╝     ╚═╝╚═╝   ╚═╝   
                                                                                                                                    
 
### git status & tracking files 
```bash
$ #on the same folder
$ cd workfolder
$ touch <NAME>.MD

$ # let's see the status after we create new file
$ git status 

$ # let's track the file
$ git add <NAME>.MD
$ git add . ## to add all files - this is folder specific

$ # let's check status
$ git status

$ # let's change file
$ vim <NAME>.MD

$ # let's see the status again
$ git status
```
 
### git reset  

```bash 
$ # to reset all staged files
$ git reset 

$ # reset specific files
$ git reset 1_GIT_SETUP.MD  
 
```
 
### git stash  

```bash 
$ # stash files to temporary location
$ git stash 

$ # retrieve files from stash
$ git stash pop

$ # list stash 
$ git stash list
$ git stash show ## more detailed
 
```


### git diff

```bash  
$ vim README.MD
$ git diff README.MD
```
 

### git log 
```bash  
$ git log 

$ # view log branch the PRETTY WAY
$ git log --all --graph --decorate --oneline

$ # or you can add to your bash profile 
$ echo "alias gitlog='git log --all --graph --decorate --oneline'" >> ~/.bash_profile
 
```