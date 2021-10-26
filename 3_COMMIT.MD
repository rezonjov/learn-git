     ██████╗ ██╗████████╗     ██████╗ ██████╗ ███╗   ███╗███╗   ███╗██╗████████╗
    ██╔════╝ ██║╚══██╔══╝    ██╔════╝██╔═══██╗████╗ ████║████╗ ████║██║╚══██╔══╝
    ██║  ███╗██║   ██║       ██║     ██║   ██║██╔████╔██║██╔████╔██║██║   ██║   
    ██║   ██║██║   ██║       ██║     ██║   ██║██║╚██╔╝██║██║╚██╔╝██║██║   ██║   
    ╚██████╔╝██║   ██║       ╚██████╗╚██████╔╝██║ ╚═╝ ██║██║ ╚═╝ ██║██║   ██║   
     ╚═════╝ ╚═╝   ╚═╝        ╚═════╝ ╚═════╝ ╚═╝     ╚═╝╚═╝     ╚═╝╚═╝   ╚═╝   
                                                                                                                                    
 
### git status & tracking files 
```bash 
$ cd workfolder
$ mkdir <NAME>
$ cd <NAME>
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
 
### git commit  

```bash  
$ git add .

$ # let's commit those files
$ git commit -m "chore: message here"

$ # let's see the log 
$ git log
```

### commit ammend  
```bash 
$ # let's say you have committed but you forgot something, you can use --amend

$ touch ANOTHER_FILE.MD
$ git commit --amend # only works if you haven't pushed

## if you have pushed, don't do --amend
``` 


### git reset  
```bash 
$ # to reset all staged files
$ git reset 

$ # reset specific files
$ git reset 1_GIT_SETUP.MD  

$ # reset hard BECAREFUL
$ git reset --hard
$ git reset --hard origin/master
 
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
$ vim 1_GIT_SETUP.MD

$ # view overall difference
$ git diff 

$ # view specific file difference`
$ git diff README.MD
```