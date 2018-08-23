# Git Cheatsheet

## Basic
```
# initialize
$ git init

# check differences from previous file
$ git diff

# check differences from specific commit history 
$ git diff <commit hash>

# check differences from specific file of specific commit history 
$ git diff <commit hash> <file>

# check the current status of current branch
$ git status

# check the history of current branch
$ git log
```

## Stage Files
```
# put untracked/edited file to the stage
$ git add <files>

# put tracked file to untracked
$ git rm <files>

# rename the tracked file
$ git mv <files>
```

## Commit Files (Take a Snapshot)
```
# commit all staged files with message
$ git commit -m "<message>"

# commit all staged files
$ git commit

# commit specific staged files
$ git commit <files>

# put all modified files to stage and commit with message
$ git commit -am "<message>"
```

## Branch
```
# check branches in local repository
$ git branch

# check branches in local and all remote sites
$ git branch -a

# create a new branch
$ git branch <new_branch_name>

# soft delete a branch
$ git branch -d <branch>

# hard delete a branch
$ git branch -D <branch>
```

## Checkout
```
# switch to the specific branch
$ git checkout <branch>

# switch to the specific commit
$ git checkout <commit hash>

# create a new branch and switch to it
$ git checkout -b <new_branch_name>

# restore a specific file to the original status of previous commit
$ git checkout <filename>

# restore all files to the original status of previous commit
$ git checkout -f
```

## Stash
```
# temporary store current change
$ git stash

# pop up previous stashed change
$ git stash pop
```

## Remote Related

### Push
```
# set upstream and push history to specific remote site and branch
$ git push -u <remote site> <branch>

# push current branch to set upstream
$ git push

# push current branch to specific remote site
$ git push <remote site>
```
### Pull
```
# clone a repository from remote 
$ git clone <url>

# update current history from upstream
$ git pull

# update current history from specific remote site
$ git pull <remote>

# update specific remote site and branch
$ git pull <remote> <branch>
```

### Remote
```
# add a new remote site
$ git remote add <name> <url>

# get the url of remote site
$ git remote get-url <name>

# set a new url to a remote site
$ git remote set-url <name> <new-url>
```