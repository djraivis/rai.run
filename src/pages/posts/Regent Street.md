---
description: Git Commands Hey
slug: Regent Street
public: true
layout: ../../layouts/BlogPost.astro
title: Git Commands and meaning
createdAt: 1676729992885
updatedAt: 1696494422859
tags: []
heroImage: /posts/Regent Street_thumbnail.jpg
---


- `init`: Initializes a new Git repository.
- `clone`: Copies an existing Git repository to a new location.
- `add`: Adds files or changes to the staging area.
- `commit`: Commits changes in the staging area to the repository.
- `push`: Uploads changes to a remote repository.
- `pull`: Downloads changes from a remote repository.
- `fetch`: Downloads changes from a remote repository, but doesn't integrate them into the local branch.
- `branch`: Lists, creates, or deletes branches.
- `checkout`: Switches to a different branch.
- `merge`: Integrates changes from one branch into another:
    - git merge [branch]-to-merge
- `reset`: Resets the repository to a previous commit.
- `log`: Shows a history of commits.
- `status`: Shows the status of files in the repository.
- `diff`: Shows differences between commits or files.
- `stash`: Temporarily saves changes that aren't ready to be committed.


`git init` initialize

`rm -fr .git` delete initial git init

`git config --global init.defaultBranch main` Change Local to Main, trunk or development

`git status` shows the list of files that are been added / modified 

`git diff` shows the inside the files the actual content

`git branch` display list of branches

`git checkout main` is switch between branches 

`git checkout -b other-branch` create other brnach


`clone` Bring a repository that is hosted somewhere like Github into a folder on your local machine

`add` Track your files and changes in Git

`commit` Save your files in Git

`push` Upload Git commits to a remote repo, like Github

`pull` Download chnages from remote repo your local machine, the opposite of push

### ~/GitHub/raivis-work main > git diff feature-readme-instructions
in this scenario **main** branch will accept changes ahead frm **feature-reaadme-instructions branch**

### ~/GitHub/raivis-work main > git merge feature-readme-instructions
this will copy and past the balck info into main branch

### ~/GitHub/raivis-work main > git branch -d feature-readme-instructions
this will delete the branch

### git commit -am "add and commit at the same time"
add and commit for the same time for the modified files

### git add . & git commit -m "Comment goes here"
add and commit

### `git reset` 
### `git reset README.md`
### `git reset HEAD~1`
options to undo

### `git log`
to display all the commits
### `git reset 8b98dfa159ae8f523eef508f7c9515a3fb8cfdd5`
this is undo the commits
### `git reset --hard 8b98dfa159ae8f523eef508f7c9515a3fb8cfdd5`
this is undo the commits and file changes as well

## `git reflog`
## `git revert 1234567`
## `git reset --hard 1234567`

## `git reset HEAD~1`

## `git reset --hard HEAD~1`
## `git push -f origin main`


### `git fetch` 
I will get all the changes that are remote repository
I weill be able to upfate my slef, and will be aware of changes


git rebase origin/main

CirlceCI

HDCPI - HDMI protected



