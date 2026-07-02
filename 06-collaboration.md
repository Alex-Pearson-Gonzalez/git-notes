# Collaboration

## Fork
A personal copy of someone else's repo on GitHub (not a terminal command — done via the GitHub website).
**When I'd use it:** Contributing to a project I don't have write access to.

## Pull Request (PR)
A GitHub feature (not a Git command) — a request to merge changes from one branch/fork into another, with room for review and discussion.

## git rebase
Replays your commits on top of another branch's latest commits, creating a cleaner, linear history (alternative to merge).
​```bash
git checkout feature-branch
git rebase main
​```
**Gotcha:** Rewrites commit history — risky on shared/public branches, best used on your own local branches before pushing.

## Merge conflicts
Happens when Git can't automatically combine changes because two branches edited the same lines differently. Git marks the conflicting section in the file:
​```
<<<<<<< HEAD
your version
=======
their version
>>>>>>> branch-name
​```
You manually edit the file to keep the correct version, then:
​```bash
git add filename.md
git commit
​```