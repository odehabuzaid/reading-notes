# Git
> Distributed Version Control System


## Table of contents

- [GIT](#GIT-Basiscs)
  - [What is GIT](#What-is-GIT)
  - [Basics](#Basics)
 

# GIT Basiscs

## What is GIT

GIT is the most common way to store and manage code versions
GIT is an open-source DVCS

there are two parts to most Git repos   
- local `repo` 
- Remote `repo`

>> A `repo` is basically just a location to store code files
---

## Basics

* Creating a Local reposotory 

`git init <Folder_Directory>`

* connect local repo to a remote (on a working project)

`git remote origin <repostory_URL>`

## Creating a Commit
---
>before pushing code to remote reposotory, we must commit changes 

**- Add files to staging area**

`git add <File_Name>` (One File)

`git add ` (Entire working directory)


**- Remove files to staging area**

`git reset <File_Name>`

**- Commit Changes**

`git commit`

`git commit -m <message>`

**- Undo commit**

`git reset HEAD` ( reset the latest commit )

`git reset HEAD index.html` ( reset specific file )


## Pull / PUSH changes to a remote reposotory 
---
> push or pull code to remote reposotory


**- Push Changes**

`git push origin <branch>`

`git pull origin <branch>`

## Using Branch
---
> Git allow us to create branches, this let us commit changes without altering the offical (`master branch`) version of the code.

**- Create a new branch**

`git branch <Branch_Name>`

**- Create and switch to a new branch**

`git checkout -b <Branch_Name>`

**- Merge your branch**

`git checkout -b <Branch_Name>` ( this can be tricky if there are conflicts)


## Other Useful Git Commands
---
```bash
# git config  - setup identity and credentials 
# git diff    - see changes between branches , repos ...
# git status  - see status of working director
# git log     - see previus commits
```


[**Back**](/../reading-notes/README.md)                     | [**TOP**](#Git) |