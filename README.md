# IEEE-Git-GitHub-Tutorial
## Table of Contents
- [Branching](#branching)
- [Pull Requests](#PR)
- [Git Commands Cheatsheet](#cmds)

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

### Staging Code

#### If you want to add all changed files (except ones that are ignored, as specified in your GitIgnore)
`git add .`

#### If you only want to add certain files
`git add <insert filename or directory>`

#### If you accidentally staged something you didn't want as part of your commit
`git restore --staged <insert filename>`

### Commiting Code
`git commit -m "<insert commit message here>"`

Make sure you always include a commit message (it should be short, to the point, and easy to read!)
