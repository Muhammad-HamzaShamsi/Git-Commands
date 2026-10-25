# 🌿 Git Commands Cheat Sheet

![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?logo=github&logoColor=white)
![Type](https://img.shields.io/badge/type-cheat%20sheet-informational)

Everyday Git commands for tracking changes, collaborating and managing projects, plus two printable cheat sheets.

📄 **Cheat sheets:** [`git-cheat-sheet.pdf`](git-cheat-sheet.pdf) · [`git-cheat-sheet-education.pdf`](git-cheat-sheet-education.pdf)

## Why Git?

- 📜 **Version tracking:** see, compare and revert every change
- 🤝 **Collaboration:** branches and pull requests let many people work in parallel
- 🔒 **Backup:** every clone is a full copy of the history

## Setup

```bash
git config --global user.name  "Your Name"
git config --global user.email "you@example.com"
git config --global init.defaultBranch main
```

## Daily workflow

```bash
git clone <url>                 # copy a repository
git status                      # what changed?
git add <file> | git add .      # stage changes
git commit -m "message"         # save a snapshot
git pull --rebase               # get latest changes
git push                        # publish commits
git log --oneline --graph       # compact history
git diff                        # unstaged changes
```

## Branching

```bash
git switch -c feature/login     # create + switch
git switch main
git merge feature/login
git rebase main                 # replay your branch on top of main
git branch -d feature/login
```

## Undo & fix

```bash
git restore <file>              # discard local changes to a file
git restore --staged <file>     # unstage
git commit --amend              # fix the last commit message/content
git revert <sha>                # new commit that undoes <sha>
git reset --soft HEAD~1         # undo last commit, keep changes staged
git stash / git stash pop       # shelve work in progress
```

## Remotes

```bash
git remote -v
git remote add origin <url>
git fetch --all --prune
git push -u origin <branch>
```
