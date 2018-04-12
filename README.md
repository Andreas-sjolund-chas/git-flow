# Git flow
## Branching

## Merging
1. git checkout <branching base>
2. git pull
3. git checkout <feature branch>
4. git rebase <branching base>
5. solve possible conflicts
6. add the solved conflicts with “git add”
7. git rebase -continue
8. repeat until step 5 - 6 until rebase is done
9. git push -f