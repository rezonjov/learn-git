# GIT INITIAL SETUP



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

### set pull strategy
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

```bash
$ git config pull.ff only 
$ git config --global pull.ff only
```
 