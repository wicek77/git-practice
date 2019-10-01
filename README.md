#Practice Repository to start learning Git


## Commmands used

- git init: Create a Repository
- git status: Compare working directory, staging area, and current branch
- git add: Add changes from working directory to staging area
- git commit: Commit changes from staging area to current branch
- git config: Set or get configuration
- git log: Show history of project commits
- git branch: list branches
- git checkout: checkout a branch (update HEAD and apply changes to working directory)
- git checkout -b: create branch, then check it out

## What's a branch?

A branch is a ref(erence) to a commit. When HEAD points to a branch, we say we're "on" that branch. When we make a commit while we're on a branch, the branch is updated to ref(er) to the new commit.

##What's a HEAD?

HEAD is a ref(erence) to the "current" branch (or sometimes a commit...more on that later). Git commands like `status`, `log`, and `branch` use HEAD. `git checkout` updates HEAD to ref(er) to a different branch.

## Commit messages


Default editor is nano (this can be changed)

Or use `git commit -m "<message>"`

- First line should be clear accurate and concise
- Use proper spelling, grammar and punctuation
- Don't end with a `.`

For more advice, see: https://chris.beams.io/posts/git-commit/
