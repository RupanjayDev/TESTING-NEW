## Git Hidden Folder

there is a hidden folder called `.git` which tells you that your project is a git repo.

If we want to create a git repo in a new project we create the folder and initialize that repo using `git init`
```
mkdir /workspaces/tmp/new-project

cd /workspaces/tmp/new-project

git init

touch Readme.md # To create readme file.

code Readme.md # To open readme file.

git status # To see what files are being tracked or untracked.
# To view changes to be committed


git add Readme_.md # To add a specific file.
git add . # git add all

# make changes to Readme.md
git commit -a -m "add readme file"

```

## CLONING
    we can clone 3 ways: hhtps, ssh, GitHub cli.

    since we are using GitHub codespaces we'll create temporary directory in our workspace.

```sh
mkdir /workspace/tmp

cd /workspace/tmp
```

### HTTPS
    git clone <http url from the local tab>
```sh
git clone https://github.com/RupanjayDev/TESTING-NEW.git 

cd TESTING-NEW

ls -la to view all the newly created directories and files that are hidden.
```

> You'll need to generate a github personel access token(PAT)

You'll use PAT as your password when you login

- Give it access to Contents for commits

### SSH


## COMMITS

when we want to commit code we can write git commit which will open up the commit edit message in the editor of choice.

```sh
git commit
```

set the global editor
```
$ git config --global core.editor emacs
```

Make commit and commit message without opening the editor
```sh
git commit -m "new change added"
```

## BRANCHES

## REMOTES

## STASHING

## MERGING

## ADD

hen we want to stage changes that will be added in the commit we can use the . to add all possible files.

```
git add Readme_.md
git add .
```

## Git RESET

Reset allow you to move staged changes to be unchanged.
This is useful when you want to revert all files not to be committed.

```
git add .
git reset
```
> git reset will revert a git add.

## GIT STATUS

git status will show you what files will or will not be committed.

```
git status
```

## GitConfig file

The gitconfig file is what stores your global configuration for git such as email, name, editor and more.

Showing contents of .gitconfig file
```
git config --list
```
when you first install git on a machine you are supposed to set up your name and email

```sh
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
```

## LOG
git log will show recent git commits to the git tree.

## PUSH
when we want to push a repo to our remote origin.

```
git push
```

## GITHUB TEMPORARY ACCESS TOKEN

```
Commit and push changes from the local environment without using credentials like email and password

GitHub personel access toke allows to just push and commit by entering username and personel access token as a password


```