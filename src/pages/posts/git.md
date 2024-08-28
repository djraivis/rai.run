---
description: To remember
slug: git
public: true
layout: ../../layouts/BlogPost.astro
title: Git Commands
createdAt: 1676729992885
updatedAt: 1724763810900
tags:
  - Git
heroImage: /posts/git_thumbnail.jpg
---

- git branch --column
- git config --global branch.sort -committerdate
- 
- 
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

<br>

```zsh
`git checkout -b P3PD-707-something-something`
`git status`
`git add -p`
`git commit -m "P3PD-707: comments comments"`
`git push -u origin  P3PD-707-something-something`
```

## Other:
- **git init**: Initialize a new Git repository.
- **git clone [repository]**: Clone a remote repository to your local machine.
- **git add [file]**: Add a file to the staging area.
- **git commit -m "message"**: Commit changes with a descriptive message.
- **git status**: View the status of files in the working directory.
- **git push**: Push local changes to a remote repository.
- **git pull**: Fetch and merge changes from a remote repository.
- **git branch**: List branches and highlight the current branch.
- **git checkout [branch]**: Switch to a different branch.
- **git merge [branch]**: Merge a branch into the current branch.
- **git diff**: Show changes between commits, branches, or files.
- **git log**: Display commit history.
- **git remote add [name] [url]**: Add a new remote repository.
- **git remote -v**: List remote repositories.
- **git stash**: Temporarily save changes that are not ready to be committed.
- **git stash pop**: Apply the most recent stash and remove it from the stack.
- **git reset [commit]**: Reset the repository to a specific commit.
- **git revert [commit]**: Revert changes made in a specific commit.
- **git fetch**: Download remote changes without merging.
- **git branch -d [branch]**: Delete a local branch.
- **git tag [name]**: Create a lightweight tag for a commit.
- **git show [commit]**: Show information about a specific commit.
- **git remote remove [name]**: Remove a remote repository.
- **git config --global user.name "name"**: Set the author name for commits.
- **git config --global user.email "email"**: Set the author email for commits.
- **git blame [file]**: Show who last modified each line of a file.
- **git fetch --prune**: Remove remote tracking branches that no longer exist on the remote.
- **git checkout -b [branch]**: Create and switch to a new branch.
- **git push --tags**: Push all tags to a remote repository.
- **git remote show [name]**: Show detailed information about a remote repository.
- **git cherry-pick [commit]**: Apply changes from a specific commit to the current branch.
- **git rebase [branch]**: Reapply commits on top of another branch.
- **git branch -r**: List remote branches.
- **git clean -n**: Show which untracked files will be removed.
- **git mv [old_path] [new_path]**: Move or rename a file.
- **git reset --hard**: Discard all changes and reset to the last commit.

<br>

```zsh
`git reset` 
`git reset README.md`
`git reset HEAD~1` - options to undo
`git log` - to display all the commits
`git reset 8b98dfa159ae8f523eef508f7c9515a3fb8cfdd5` - this is undo the commits
`git reset --hard 8b98dfa159ae8f523eef508f7c9515a3fb8cfdd5` - this is undo the commits and file changes as well
```

<br>

- **git log --author="name"**: Show commits by a specific author.
- **git branch -a**: List all branches, local and remote.
- **git diff [branch1] [branch2]**: Show differences between two branches.
- **git show-branch**: Show branches and their commits.
- **git config --global alias.[alias_name] [command]**: Create a custom Git alias.
- **git fetch --all**: Fetch all remote branches.
- **git bisect**: Find the commit that introduced a bug.
- **git cherry-pick --continue**: Continue a cherry-pick operation after resolving conflicts.
- **git commit --amend**: Amend the last commit with new



