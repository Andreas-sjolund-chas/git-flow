# Git flow

## Naming

  ### Feature-branches
  Are named after the following standard: `feature/branch-name`

  > Example: `feature/button-default` || `feature/input-primary`

  ### Hotfix-branches
  Are named after the following standard: `hotfix/branch-name`

  > Example: `hotfix/button-typo` || `hotfix/link-broken`

## Branching
1. `git pull` - Always do this to make sure you're up to date
2. `git checkout -b <feature/branch-name>`

## Merging
1. `git checkout <base-branch>`
2. `git pull`
3. `git checkout <feature/branch-name>`
4. `git rebase <base-branch>`
5. `solve possible conflicts`
6. `add the solved conflicts with “git add”`
7. `git rebase -continue`
8. `repeat until step 5 - 6 until rebase is done`
9. `git push -f`

**NOTE:** Always make sure to assign reviewers when creating a new pull request no matter how big or small your changes are.

## Managing branches
> Renaming the current branch:

`git branch -m <new-name>`

> Renaming a branch while currently not in the branch to be renamed:

`git branch -m <old-name> <new-name>`

> Deleting local branch:

`git branch -d <branch-name>`