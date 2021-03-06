# studygit

## working with branch
* create branch
```
git branch new_branch
git checkout new_branch
/* or */
git checkout -b new_branch
```
* get branch from remote
```
git fetch origin
git checkout -t -b new_branch_name_to_create origin/remote_branch_name

/* To push back, simply use git push because we already make remote tracking from git checkout above */
git push
```
* delete local branch
```
git branch -d branch_name

/* or to force delete */
git branch -D branch_name
```
* delete remote branch
```
git push origin --delete branch_name
```
* get local update from upstream
```
git pull upstream master

/* after that if you want to update to remote repo just do */
git push
```

## logging
* show commit log
```
git log --oneline --graph --decorate --all
```

## reset
* reset a specific file to the last-committed state/discard uncommitted changes
```
git checkout file_name
```
* reset the entire repository to the last committed state
```
rm file_name
git reset --hard HEAD~1
or
git reset --hard HEAD^

/* to update remote repo after reset*/
git push -f
```
* remove untracked files
```
git clean -d -x -f
```

## working with remote url
* Change remote url
```
git remote set-url origin new_url_name
```





