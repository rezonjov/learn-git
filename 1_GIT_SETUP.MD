 
    ██╗███╗   ██╗██╗████████╗██╗ █████╗ ██╗         ███████╗████████╗███████╗██████╗ 
    ██║████╗  ██║██║╚══██╔══╝██║██╔══██╗██║         ██╔════╝╚══██╔══╝██╔════╝██╔══██╗
    ██║██╔██╗ ██║██║   ██║   ██║███████║██║         ███████╗   ██║   █████╗  ██████╔╝
    ██║██║╚██╗██║██║   ██║   ██║██╔══██║██║         ╚════██║   ██║   ██╔══╝  ██╔═══╝ 
    ██║██║ ╚████║██║   ██║   ██║██║  ██║███████╗    ███████║   ██║   ███████╗██║     
    ╚═╝╚═╝  ╚═══╝╚═╝   ╚═╝   ╚═╝╚═╝  ╚═╝╚══════╝    ╚══════╝   ╚═╝   ╚══════╝╚═╝     
                                                                                 


### set your identity
```bash 
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
```

### set editor
```bash
$ git config --global core.editor vim
```

### set git main branch
```bash
$ git config --global init.defaultBranch main
```

### view applied config
```bash
$ git config --list
$ git config user.name
```

### IMPORTANT: set pull strategy 
```bash
$ git config pull.ff only 

$ # to set globally
$ git config --global pull.ff only
```
```bash
$ hint: Pulling without specifying how to reconcile divergent branches is
$ hint: discouraged. You can squelch this message by running one of the following
$ hint: commands sometime before your next pull:
$ hint: 
$ hint:   git config pull.rebase false  # merge (the default strategy)
$ hint:   git config pull.rebase true   # rebase
$ hint:   git config pull.ff only       # fast-forward only
$ hint: 
$ hint: You can replace "git config" with "git config --global" to set a default
$ hint: preference for all repositories. You can also pass --rebase, --no-rebase,
$ hint: or --ff-only on the command line to override the configured default per
$ hint: invocation.
```

 

### Optional: Install bash completion
```bash
$ #ubuntu
$ sudo apt install bash-completion


$ #mac
$ brew install bash-completion
$ echo "[ -f /usr/local/etc/bash_completion ] && . /usr/local/etc/bash_completion" >> ~/.bash_profile
$ source ~/.bash_profile ## or ~/.zsh_profile


$ #windows
$ mkdir ~/bash_completion.d    
$ curl -o ~/bash_completion.d/git https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash
$ echo "source ~/bash_completion.d/git" >> ~/.bashrc
```

