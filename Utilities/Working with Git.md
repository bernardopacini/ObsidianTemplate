---
tags:
  - git
  - it
---
## Setup

```bash
git init                    # Initialize a repository
git clone <url>             # Clone a repository
git config --list           # View Git configuration
```

## Check Status & Changes

```bash
git status                  # Check working tree status
git diff                    # View unstaged changes
git diff --staged           # View staged changes
git log --oneline           # View compact commit history
```

## Stage & Commit

```bash
git add <file>              # Stage a file
git add .                   # Stage all changes
git restore <file>          # Discard changes to a file
git restore --staged <file> # Unstage a file
git commit -m "message"     # Create a commit
git commit --amend          # Modify the latest commit
```

## Branches

```bash
git branch                  # List branches
git switch <branch>         # Switch branches
git switch -c <branch>      # Create and switch to a branch
git branch -d <branch>      # Delete a branch
```

## Remote Repositories

```bash
git remote -v               # View remotes
git fetch                   # Download remote changes
git pull                    # Fetch and merge remote changes
git push                    # Push commits
git push -u origin <branch> # Push branch and set upstream
```

## Merge & Rebase

```bash
git merge <branch>          # Merge a branch
git rebase <branch>         # Rebase onto a branch
```

## Undo

```bash
git revert <commit>         # Create a commit that undoes a commit
git reset --soft HEAD~1     # Undo commit, keep changes staged
git reset --mixed HEAD~1    # Undo commit, keep changes unstaged
git reset --hard HEAD~1     # Undo commit and discard changes
```

Tip: Be cautious with reset --hard — discarded changes may be difficult or impossible to recover.