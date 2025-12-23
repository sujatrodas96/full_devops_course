# Reset / Revert / Rebase / Merge

# Merge
1. git merge <branch> -- Merge branch into current

# Rebase
2. git rebase <branch> -- Rewrite history to linear
3. git rebase -i HEAD~n -- Interactive rebase

# Reset (Undo commits)
4. git reset --soft HEAD~1 -- Undo commit keep staged
5. git reset --mixed HEAD~1 -- Undo commit unstage
6. git reset --hard HEAD~1 -- Undo commit + delete changes

# Revert
7. git revert <commit> -- Safe undo without losing history
