     ██████╗ ██╗████████╗    ██████╗  █████╗ ███████╗██╗ ██████╗
    ██╔════╝ ██║╚══██╔══╝    ██╔══██╗██╔══██╗██╔════╝██║██╔════╝
    ██║  ███╗██║   ██║       ██████╔╝███████║███████╗██║██║     
    ██║   ██║██║   ██║       ██╔══██╗██╔══██║╚════██║██║██║     
    ╚██████╔╝██║   ██║       ██████╔╝██║  ██║███████║██║╚██████╗
     ╚═════╝ ╚═╝   ╚═╝       ╚═════╝ ╚═╝  ╚═╝╚══════╝╚═╝ ╚═════╝
                                                            

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

### git log 
```bash  
$ git log 

$ # view log branch the PRETTY WAY
$ git log --all --graph --decorate --oneline

$ # or you can add to your bash profile 
$ echo "alias gitlog='git log --all --graph --decorate --oneline'" >> ~/.bash_profile
```

### remote
```bash
# list git remote
$ git remote -v

# add remote repository
$ git remote add <name> <url>
$ git remote -v
 
# delete remote repository
$ git remote remove <name>

# update repo from all remote update
$ git remote update
```

### pull
```bash
$ git fetch # updates remote files
$ git pull # update remote files and do merge

$ # pull from specific remote 
$ git pull <remote> 

$ # pull from specific remote branch 
$ git pull <remote> <branch>

$ # Try-me: 
$ git checkout main
$ git pull origin final  # what happens? 
``` 