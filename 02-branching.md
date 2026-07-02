# Branching

A branch is basically an independent line of development — a separate path of commits that lets you work on something without touching the main version of your code.

## git branch
Lists, creates, or deletes branches.
​```bash
git branch                # list branches
git branch new-feature    # create a branch
git branch -d old-feature # delete a branch (safe, only if merged)
git branch -D old-feature # force delete (even if unmerged)
​```
**Gotcha:** Creating a branch doesn't switch you to it.

## git checkout
Switches between branches, or restores files. Older, more multi-purpose command.
​```bash
git checkout branch-name        # switch to a branch
git checkout -b new-branch      # create AND switch in one step
​```

## git switch
Newer, cleaner command just for switching branches (does one job, not several).
​```bash
git switch branch-name          # switch to a branch
git switch -c new-branch        # create AND switch
​```

## git merge
Combines changes from one branch into another.
​```bash
git checkout main
git merge feature-branch
​```
**When I'd use it:** Bringing finished feature work back into `main`.
**Gotcha:** Can cause merge conflicts if both branches changed the same lines.