# History

## git log
Shows commit history — hash, author, date, message.
​```bash
git log
git log --oneline          # condensed, one line per commit
git log --oneline --graph  # visual branch/merge structure
​```

## git diff
Shows exact line-by-line changes.
​```bash
git diff                   # unstaged changes vs last commit
git diff --staged          # staged changes vs last commit
git diff branch1 branch2   # differences between two branches
​```

## git blame
Shows who last changed each line of a file, and in which commit.
​```bash
git blame filename.md
​```
**When I'd use it:** Figuring out who/why a specific line was written, e.g. tracking down a bug's origin.

## git show
Shows the full details (diff + metadata) of a specific commit.
​```bash
git show <commit-hash>
​```