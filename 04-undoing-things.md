# Undoing Things

## git restore
Discards changes in your working directory (before staging).
​```bash
git restore filename.md
​```

## git restore --staged
Unstages a file (keeps the edits, just removes it from "ready to commit").
​```bash
git restore --staged filename.md
​```

## git reset
Moves your branch pointer backward, undoing commits.
​```bash
git reset --soft HEAD~1   # undo last commit, keep changes staged
git reset --mixed HEAD~1  # undo last commit, keep changes unstaged (default)
git reset --hard HEAD~1   # undo last commit, DELETE the changes entirely
​```
**Gotcha:** `--hard` is destructive — changes are gone, not recoverable easily.

## git revert
Creates a NEW commit that undoes a previous commit — doesn't rewrite history.
​```bash
git revert <commit-hash>
​```
**When I'd use it:** Undoing something that's already been pushed/shared — safer than `reset` in that case.

## git checkout -- file
Older syntax for discarding changes to a specific file (mostly replaced by `restore`).
​```bash
git checkout -- filename.md
​```