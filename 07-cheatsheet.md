# Quick Command Cheatsheet

| Command | Purpose |
|---|---|
| `git init` | Start a new repo |
| `git clone <url>` | Copy a remote repo locally |
| `git status` | See what's changed |
| `git add <file>` | Stage changes |
| `git commit -m "msg"` | Save a snapshot |
| `git push` | Upload commits to GitHub |
| `git pull` | Download + merge latest changes |
| `git branch` | List/create/delete branches |
| `git switch <branch>` | Change branches |
| `git switch -c <branch>` | Create + switch to new branch |
| `git merge <branch>` | Combine branches |
| `git remote -v` | Show connected remotes |
| `git fetch` | Download changes without merging |
| `git restore <file>` | Discard unstaged changes |
| `git restore --staged <file>` | Unstage a file |
| `git reset --soft HEAD~1` | Undo last commit, keep changes staged |
| `git reset --hard HEAD~1` | Undo last commit, delete changes |
| `git revert <hash>` | Undo via a new commit (safe for shared history) |
| `git log --oneline --graph` | View commit history visually |
| `git diff` | See exact changes |
| `git blame <file>` | See who changed each line |
| `git show <hash>` | See full details of a commit |
| `git rebase <branch>` | Replay commits for linear history |