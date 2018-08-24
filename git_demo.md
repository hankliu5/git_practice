# Git Demo

## Demo 1: Create a Local Repository

```shell
$ mkdir git_solo
$ cd git_solo

# Initialize the git repository
$ git init

$ echo "hello, world" >> test.txt

# check the status of repository
$ git status

# put untracked file to the stage
$ git add test.txt

$ git status

# take a snapshot of staged files
$ git commit -m "first commit."

$ git status

### use vim to edit test.txt ###

$ git status

# check the difference from previous commit
$ git diff

$ git add test.txt
$ git status
$ git commit -m "second commit."
$ git status

# check the history of current branch
$ git log
```

## Demo 2: Create a Remote Repository
Create a new repository on GitHub

```shell
# link remote url to local repository
$ git remote add origin git@github.com:hankliu5/git_practice.git

# Set a new branch on remote and push the history to remote
$ git push -u origin master
```

## Demo 3-1: Collaborate with Others
```shell
$ cd

# clone a repository from remote
$ git clone git@github.com:ESCALNCSU/GitPractice.git
$ cd GitPractice

# check all branch information of repository
$ git branch -a

# switch to dev branch
$ git checkout dev

# create a new branch from dev
$ git checkout -b <your name>

### use editor to edit the file with your name ###

$ git add <file with your name>
$ git commit -m "<commit message>"
$ git push -u origin <your branch name>
```

## Demo 4-1: Pull Request
1. Go to https://github.com/ESCALNCSU/GitPractice
2. Click **[new pull request]**
3. Choose base as `dev`
4. Choose compare as `<your branch>`
5. Click **[Create pull request]**

## Demo 4-2: Update the Shared Branches
```shell
$ git checkout dev

# update the history of dev branch
$ git pull

$ git checkout <your branch>

# merge the history of dev branch to current branch
$ git merge dev
$ git status
```

## Demo 5: Fix Conflicts
```shell
### use editor to edit the conflicted file
### search "===="
### choose what to keep and what to discard
### save the file

$ git add <the conflicted file>
$ git commit -m "fix the conflict"
$ git push
```




