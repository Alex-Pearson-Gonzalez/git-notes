# Remotes

## git remote -v
Shows which remote URLs your local repo is connected to.
​```bash
git remote -v
​```
Typically shows `origin` — the default name for "the repo I cloned from."

## git fetch
Downloads new commits from the remote, but does NOT merge them into your current branch.
​```bash
git fetch origin
​```
**When I'd use it:** To see what's changed on GitHub before deciding whether to pull it in.

## origin
The default nickname Git gives to the remote repo you cloned from. Not a command — just a label.
​```bash
git push origin main
​```

## upstream
Used when you've forked someone else's repo. `origin` = your fork, `upstream` = the original repo you forked from.
​```bash
git remote add upstream https://github.com/original-owner/repo.git
git fetch upstream
​```