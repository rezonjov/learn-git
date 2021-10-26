     ██████╗ ██╗████████╗    ███╗   ███╗███████╗██████╗  ██████╗ ███████╗
    ██╔════╝ ██║╚══██╔══╝    ████╗ ████║██╔════╝██╔══██╗██╔════╝ ██╔════╝
    ██║  ███╗██║   ██║       ██╔████╔██║█████╗  ██████╔╝██║  ███╗█████╗  
    ██║   ██║██║   ██║       ██║╚██╔╝██║██╔══╝  ██╔══██╗██║   ██║██╔══╝  
    ╚██████╔╝██║   ██║       ██║ ╚═╝ ██║███████╗██║  ██║╚██████╔╝███████╗
     ╚═════╝ ╚═╝   ╚═╝       ╚═╝     ╚═╝╚══════╝╚═╝  ╚═╝ ╚═════╝ ╚══════╝
                                                                     


```
Sometimes we need to update our local branch with remote branch. In general, there are 2 strategies to do that. We can do `merge` or `rebase`
```



> **Typical use case:** We want to create Merge Request. Before we do so, we need to make sure our local branch is updated from master.  



## git merge 
```bash
$ # let's say we want to merge branch `main` to branch `A`. We need to checkout branch A
$ git checkout A

$ # make sure the local `main` branch is up to date
$ git fetch origin main

$ # then let's merge
$ git merge main 
```


## git rebase
```bash
$ # let's say we want to update branch `A` with branch `main`. We need to checkout branch A
$ git checkout A

$ # make sure the local `main` branch is up to date
$ git fetch origin main

$ # then let's merge
$ git rebase main 
```



## git squash all into 1 commit
```bash
$ # let's say we want to squash all commit into one. There are 2 options

# Option 1 - use Rebase
$ git rebase -i HEAD~X
$ # OR
$ git rebase -i <COMMIT_REF>


---

# Option 2 - use Reset Soft

$ git reset --soft HEAD~X
$ git add .
$ git commit -m "combine: message commit"
$ git push +main
```
