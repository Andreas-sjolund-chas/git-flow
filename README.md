# Git flow
## Branching
1. git pull **Always do this to make sure you're up to date**
2. git checkout -b `<feature-branch-name>`

## Merging
1. git checkout `<base-branch>`
2. git pull
3. git checkout `<feature-branch>`
4. git rebase `<base-branch>`
5. solve possible conflicts
6. add the solved conflicts with “git add”
7. git rebase -continue
8. repeat until step 5 - 6 until rebase is done
9. git push -f