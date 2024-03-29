#Practice Repository to start learning Git


## Commmands used

- git init: Create a new Git Repository
- git status: Compare working directory, staging area, and current branch
- git add: Add changes from working directory to staging area
- git commit: Commit changes from staging area to current branch
- git config: Set or get configuration
- git log: Show a history (aka "logs") of project commits
- git branch: list branches
- git branch -c: Creates a branch
- git checkout: checkout a branch (update HEAD and apply changes to working directory)
- git checkout -b: create branch, then check it out
- git show: Shows detailed info on a single commit
- git diff: Shows differences in what changes have been made. Can be used for changes in stging area, compare branches, as well as last change on a single branch
- git merge: Merge changes from different branches
- git stash: Stash changes from working directory
- git stash list: List stashes
- git stash pop: Apply stashed changes to working directory
- git remote add <remote> <url>: Add a new <remote> at <url>
- git remote -v: List remote repositories
- git push -u <remote> <branch(master)>: Push <branch> to <remote> and set default upstream for <branch>
- git fetch: Fetch changes from remote repository
- git pull: Fetch, and then merge

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

## Merging

Merging means to bring the changes from one branch to another.

- A fast-forward merge happens when the target branch was branched from the current one, and there are no new changes to the current branch since then.
- An Automatic merge happens when the two histories have diverged, but git is able to reconcile them into one set of changes. This creates a new commit on the current branch.

## What's a remote?

A remote repository is one hosted somewhere other than our local machine. We can add remotes with `git remote add`, and set up *tracking branches* to track differences between our local and remote repositories.

We push to remotes with `git push`, and fetch from them with `git fetch`. We can also fetch and merge in one set with `git pull`
