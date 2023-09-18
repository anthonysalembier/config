##Git global config

> 
    [user]
        name = Anthony Salembier
        email = e@mail.com

    [alias]
        aliases =! git config -l | grep alias | cut -c 7-
        ca = commit --amend --all -C HEAD
        cod = checkout origin/develop
        com = checkout origin/main
        cp = cherry-pick
        dead =! git add . && git commit --amend --all -C HEAD && git push --force-with-lease
        f = fetch --prune --prune-tags --force
        fuck =! git add . && git stash && git stash clear
        please = push --force-with-lease
        rod = rebase origin/develop
        rom = rebase origin/main
        rup = remote update --prune
        s = status
        tej = "!sh -c 'git tag -d $0 && git push --delete origin $0 --force'"
        tree = log --graph --decorate --pretty=oneline --abbrev-commit --all
        wipe = "!sh -c 'git branch -D $0 && git push --delete origin $0'"
