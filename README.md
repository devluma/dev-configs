# dev-configs
Settings for development in operating systems (WINDOWS, MAC and LINUX)

# GIT

```
[user]
	email = <seu e-mail>
	name = <seu nome>

[alias]
    ci = "!f() { git commit -m \"$*\"; }; f"
    co = checkout
    cm = checkout master
    cb = checkout -b
    ckd = checkout -b develop
    fet = fetch 
    st = status -sb
    sf = show --name-only
    lg = log --pretty=format:'%Cred%h%Creset %C(bold)%cr%Creset %Cgreen<%an>%Creset %s' --max-count=30
    incoming = !(git fetch --quiet && git log --pretty=format:'%C(yellow)%h %C(white)- %C(red)%an %C(white)- %C(cyan)%d%Creset %s %C(white)- %ar%Creset' ..@{u})
    outgoing = !(git fetch --quiet && git log --pretty=format:'%C(yellow)%h %C(white)- %C(red)%an %C(white)- %C(cyan)%d%Creset %s %C(white)- %ar%Creset' @{u}..)
    pum = pull origin master
    pud = pull origin develop
    pl = pull
    pom = push origin master -u
    pod = push origin develop -u
    ps = push
    unstage = reset HEAD --
    undo = checkout --
    rollback = reset --soft HEAD~1
```
