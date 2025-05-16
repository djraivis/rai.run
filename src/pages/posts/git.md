---
description: null
slug: git
public: true
layout: ../../layouts/BlogPost.astro
title: 🌱 Git Aliases Cheat Sheet
createdAt: 1676729992885
updatedAt: 1746600373616
tags:
  - Git
heroImage: /posts/git_thumbnail.jpg
---


## 🔹 Status & Branches
- `gs` → git status  
- `gst` → git status -sb  
- `gb` → git branch  
- `gbr` → current branch name  
- `gco` → git checkout  
- `gcl` → git clone  

## 🔹 Add & Commit
- `ga` → git add  
- `gaa` → git add .  
- `gcm "msg"` → git commit -m "msg"  
- `gcam "msg"` → git commit -am "msg"  
- `gca` → git commit --amend  
- `gcan` → git commit --amend --no-edit  

## 🔹 Push & Pull
- `gp` → git push  
- `gpu` → git push -u origin HEAD  
- `gpo` → git push origin  
- `gpl` → git pull --rebase  

## 🔹 Diff, Restore, Reset
- `gd` → git diff  
- `gr` → git restore  
- `grs` → git restore --staged .  
- `greset` → git reset  
- `grhh` → git reset --hard HEAD  
- `gundo` → git reset --soft HEAD~1  

## 🔹 Logs & Blame
- `gl` → git log --oneline --graph --decorate --all  
- `glog` → same as above  
- `gbl` → git blame -w -M -C  

## 🔹 Stash
- `gstash` → git stash  
- `gstashp` → git stash pop  
- `gstashl` → git stash list  

## 🔹 Tags & Submodules
- `gtag` → git tag  
- `gtags` → git tag -n  
- `gsu` → git submodule update --init --recursive  

## 🔹 Delete
- `gbd` → git branch -d  
- `gbD` → git branch -D  
- `gbrd NAME` → git push origin --delete NAME  

## 🔹 Misc
- `gcp` → git cherry-pick  
- `grevert` → git revert  
- `gurl` → show repo remote URL  

---


## Git Commands Meanings

- `git branch --column`
- `git config --global branch.sort -committerdate`
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
- `reset`: Resets the repository to a previous commit.
- `log`: Shows a history of commits.
- `status`: Shows the status of files in the repository.
- `diff`: Shows differences between commits or files.
- `stash` - Temporarily saves changes that aren't ready to be committed.
- `git init` initialize
- `rm -fr .git` delete initial git init
- `git config --global init.defaultBranch main` Change Local to Main, trunk or development
- `git status` shows the list of files that are been added / modified 
- `git branch` display list of branches
- `git checkout main` is switch between branches 
- `git checkout -b other-branch` create other brnach

```zsh
`git checkout -b P3PD-707`
`git status`
`git add -p`
`git commit -m "P3PD-707: comments comments"`
`git push -u origin  P3PD-707-something-something`
```

