     ██████╗ ██╗████████╗    ██████╗ ██████╗  █████╗ ███╗   ██╗ ██████╗██╗  ██╗
    ██╔════╝ ██║╚══██╔══╝    ██╔══██╗██╔══██╗██╔══██╗████╗  ██║██╔════╝██║  ██║
    ██║  ███╗██║   ██║       ██████╔╝██████╔╝███████║██╔██╗ ██║██║     ███████║
    ██║   ██║██║   ██║       ██╔══██╗██╔══██╗██╔══██║██║╚██╗██║██║     ██╔══██║
    ╚██████╔╝██║   ██║       ██████╔╝██║  ██║██║  ██║██║ ╚████║╚██████╗██║  ██║
     ╚═════╝ ╚═╝   ╚═╝       ╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═══╝ ╚═════╝╚═╝  ╚═╝
                                                                           
### create new branch
```bash
$ git checkout main 

$ git pull # make sure you are on the latest commit

$ # let's create a new branch `branch-name`
$ git checkout -b branch-name


$ # see the branch again
$ git branch -v
```

### rename a branch
```bash
$ git branch -m newnamehere\

## try to pull and see the error
```


### delete a branch
```bash
$ git checkout main

<<<<<<< Updated upstream
$ # delete `branch-name`
$ git branch -D branch-name
=======
$ # delete local `branch-name` 
$ git branch -D branch-name 


$ # delete remote `branch-name` 
$ git push origin --delete branch-name 
>>>>>>> Stashed changes
```

