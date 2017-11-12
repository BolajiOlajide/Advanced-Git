## What is a Branch?
A branch is simply a pointer to a particular commit

## What is HEAD?
It is how git knows what branch you're currently on. It is how git knows what the parent of the next commit will be. It usually points to the name of the current branch.

## What is a tag?
A tag is simply a pointer to a commit.

## Difference between a tag and a branch
For a branch, the current branch pointer moves with every commit to the repository.
For a tag, the commit a tag points to doesn't change, it's a snapshot.

## Headless State (or detached head state)
This occurs when you need to checkout to a specific commit instead of a branch. Git moves the HEAD pointer to that commit. If you want to save work done in a detached head state, simply create a new branch that points to the last commit made in that state.

`git branch <new-branch-name> <last-commit>`

## Dangling Commits
These are commits that are made in a headless state. They don't point to any branch and because of that can't be referenced in git. They are usually garbage collected after a period of time.

## Merge Conflicts
These occur when we try to merge but our files have diverged. Git stops until the conflicts are resolved.

## Git RERERE (Reusable Recoreded Resolution)
It is a way git saves the way you resolved a merge conflict and tries to reuse for any more conflicts that might occur.

## Fastforward Commits
Fast forward commits happen when the base branch (the one you created your branch on) hasn't changed after you branched from it. The history is linear.
