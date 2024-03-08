# Git

Git is a distributed version control system that enables collaborative software development by tracking changes to source code, facilitating team coordination, and preserving project history.

test

---
## Basic commands

```bash
# Initialize a Git repository
git init --initial-branch=main

# Check repository status
git status

# Add changes to the staging area
git add <file_name>
git add .

# Commit changes
git commit -m "Commit message"

# Fetch changes from all remotes
git fetch --all

# Rebase the current branch onto another branch
git rebase <branch_name>
```
---
## Branching

```bash
# Create a new branch
git branch <branch_name>

# Switch to a branch
git checkout <branch_name>

# Create and switch to a new branch
git checkout -b <branch_name>

# Merge a branch into the current branch
git merge <branch_name>

# Delete a branch
git branch -D <branch_name>
```
---
## Remote Repositories

```bash
# Check remote origin
git remote -v

# Change remote origin
git remote set-url <remote_name> <remote_url>

# Add remote origin
git remote add <remote_name> <remote_url>

# Push changes to a remote repository
git push <remote_name> <branch_name>

# Pull changes from a remote repository
git pull <remote_name> <branch_name>
```
---
## Reverting Changes

```bash
# Revert a commit
git revert <commit_hash>

# Undo unstaged changes in a file
git checkout -- <file_name>
```
---
## Miscellaneous

```bash
# Remove folder from Git
git rm -r --cached <path/to/folder>

# Show commit history
git log

# Show changes between commits
git diff <commit1> <commit2>

# Discard changes in the working directory
git checkout -- <file_name>

# Undo the last commit but keep changes
git reset --soft HEAD^

# Amend the last commit
git commit --amend -m "New commit message"

# List all branches
git branch

# Show changes staged for the next commit
git diff --staged

# Show the difference between branches
git diff <branch1> <branch2>

# Tagging a commit
git tag -a <tag_name> -m "Tag message" <commit_hash>

# List all tags
git tag
```