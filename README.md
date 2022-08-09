# Git Configuration

My git configuration. To be placed in global or local git config.

    [alias]
        c = commit
        co = checkout
        st = status
        br = branch
        hist = log --pretty=format:'%h %ad | %s%d [%an]' --graph --date=short
        cp = cherry-pick
        load = !git push origin HEAD
        undo = !git reset HEAD~1 && git st
        fix = !git commit --amend --no-edit && git st
        fixa = !git add . && git commit --amend --no-edit && git st
        tmp = !git commit -m "tmp" && git st
        tmpa = !git add . && git commit -m "tmp" && git st
        drop = !git add . && git reset --hard
        dropo = !git add . && git reset --hard origin/HEAD
