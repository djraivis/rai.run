---
description: To remember
slug: git
public: true
layout: ../../layouts/BlogPost.astro
title: Git Commands
createdAt: 1676729992885
updatedAt: 1724946376613
tags:
  - Git
heroImage: /posts/git_thumbnail.jpg
---

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




