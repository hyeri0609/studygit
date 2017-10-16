# studygit

## working with branch
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
