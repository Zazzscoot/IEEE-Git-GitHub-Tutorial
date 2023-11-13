# IEEE-Git-GitHub-Tutorial
## Table of Contents
- [Branching](#branching)
- [Pull Requests](#PR)
- [Git Commands Cheatsheet](#cmds)
- [Dealing with Merge Conflicts](#mcs)

## Branching

## Pull Requests

<a id="cmds"></a>
## Git Commands Cheatsheet
### Setup
#### If you have a remote GitHub repository already

Clone a repository

`git clone <insert GitHub Repository link here>`

---
#### If you are starting locally (i.e. you have some code already, and you want to push it to a repository)

Initialize an empty local repository

`git init`

Set the remote branch (i.e. where we want to push the code to)

`git remote add origin <insert GitHub Repository link here>`

### Making a new branch
`git checkout -b <insert branch name>`

It is super important for you to make a new branch (with a new name that doesn't exist yet on the GitHub repository), so that you have a working copy on your local repository!
### Staging Code

#### If you want to add all changed files (except ones that are ignored, as specified in your GitIgnore)
`git add .`

#### If you only want to add certain files
`git add <insert filename or directory>`

#### If you accidentally staged something you didn't want as part of your commit
`git restore --staged <insert filename>`

### Commiting Code
`git commit -m "<insert commit message>"`

Make sure you always include a commit message (it should be short, to the point, and easy to read!)

### Pushing Code to GitHub
#### If you are pushing code for the first time on the branch you are currently on

i.e. (This is the first time you are pushing since the last time you did `git checkout -b <insert branch name>`)

`git push --set-upstream origin <insert your branch name>`

IMPORTANT: make sure the branch name you put here is the same as what your branch is called locally!

#### If you are NOT pushing code for the first time on the branch
`git push`

<a id="mc"></a>
## Dealing with Merge Conflicts

This is very likely to happen when you make a pull request, especially if you are working on a collaborative project!

To deal with this, you can merge your code locally. First, let's pull the code on the main branch currently.

`git pull origin main`
