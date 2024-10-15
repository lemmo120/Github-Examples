## Git Hidden Folder

There is a hidden folder called `.git` which tells you that your project is a git repo.

If we wanted to create a git repo in a new project we'd create the folder and then initialise that repo using `git init`

```
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
code Readme.md
git status
git add Readme.md
# make changes to readme.md
git commit -m "add readme file"
```

## Cloning

We can clone three ways: HTTPS, SSH, Github CLI

Since we are using GitHub codespaces we'll create a temporary directory in our workspace

```sh
mkdir /workspace/tmp
cd /workspace/tmp
```

### HTTPS

```sh 
git clone https://github.com/lemmo120/Github-Examples.git
cd GitHub-Examples
```

> You'll need to generate a Personal Access Token (PAT)
You will use the PAT as your password when you login

- Give it access to Contens for commits



## Commits

When we want to commit code we can write git commit which will open up the commit edit message in the editor of choice.

``` sh
git commit
```

Make a commit and commit message without opening an editor
```sh
git commit -m "add another !"
```

## Log

git log will show recent git commits to the git tree

## Push

When we want to push a repo to our remote origin

```
git push
```

## Branches

## Remotes

## Stashing

## Merging

## Add

When we want to stage changes that will be included in the commit. We can use the . to add all possible files.

``` 
git add Readme.md
git add .
```

## Status

Git status shows you what files will or will not be commited.

```
git status
```

## Reset

Reset allows you to move Staged changes to be unstaged.
This is useful when you want to revert all files not to be commited. 

``` 
git add .
git reset
```

> git reset will revert a git add

## Gitconfig file

The gitconfig file is what sotres your global configurations for git such as name, email, editor and more

Showing the contents of our .gitconfig file
```
git config --list
```