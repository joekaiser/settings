
[alias]
        lg = log
        ls = log --pretty=format:"%ci\\ %C(yellow)%h%Cred%d\\ %Creset%s%Cblue\\ [%cn]" --decorate
        ll = log --pretty=format:"%ci\\ %C(yellow)%h%Cred%d\\ %Creset%s%Cblue\\ [%cn]" --decorate --numstat
        co = checkout
        ci = commit
        st = status
        wipe = !git add -A && git commit -qm 'WIPE SAVEPOINT' && git reset HEAD~1 --hard
        release = !git checkout release && git pull && git merge master && git push && git checkout master
