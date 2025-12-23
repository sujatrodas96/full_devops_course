======================== COMPLETE GIT COMMANDS WITH PURPOSE ========================

1. git init -- To initialize an empty Git repository

2. git status -- To check current repo status (tracked, untracked, staged files)

3. git add . -- To stage all files
4. git add <file> -- To stage a specific file
5. git add *.ext -- To stage files based on pattern

6. git commit -m "msg" -- To commit staged files with a message
7. git commit -am "msg" -- To add + commit tracked files directly

8. git push -- To push commits to remote repository
9. git push origin main -- To push code to main branch
10. git push -u origin main -- To set upstream and push

11. git restore -- To discard working directory changes
12. git restore <file> -- To discard a file's changes
13. git restore --staged <file> -- To unstage a staged file

14. git revert <commit_id> -- To undo commit safely by creating a new commit

15. git log -- To see full commit history
16. git log --oneline -- To see compact commit history
17. git log --graph --decorate --oneline --all -- To see visual commit history tree

18. git branch -- To list all branches
19. git branch <name> -- To create a new branch
20. git branch -d <name> -- To delete merged branch safely
21. git branch -D <name> -- To force delete branch

22. git checkout <branch> -- To switch to a branch
23. git checkout -b <branch> -- To create + switch to branch

24. git switch <branch> -- To switch branch (modern safer command)
25. git switch -c <branch> -- To create + switch branch

26. git merge <branch> -- To merge branch into current branch

27. git rebase <branch> -- To rewrite history & make linear commits
28. git rebase -i HEAD~n -- To interactively edit commits

29. git pull -- To fetch + merge updates from remote
30. git pull origin main -- To pull from main branch
31. git pull --rebase -- To pull updates by rebasing

32. git fetch -- To download changes without merging
33. git fetch origin -- To fetch from origin remote

34. git cherry-pick <commit> -- To copy a specific commit to another branch

===================== RESET (UNDO COMMANDS) =====================

35. git reset --soft HEAD~1 -- To undo commit but keep changes staged
36. git reset --mixed HEAD~1 -- To undo commit & unstage files
37. git reset --hard HEAD~1 -- To undo commit and delete changes (dangerous)

===================== STASH (TEMPORARY SAVE) =====================

38. git stash -- To temporarily save uncommitted work
39. git stash list -- To view saved stashes
40. git stash pop -- To restore latest stash and remove it
41. git stash apply -- To restore stash without deleting
42. git stash drop -- To delete a stash
43. git stash clear -- To delete all stashes

===================== DIFF (COMPARE CHANGES) =====================

44. git diff -- To show unstaged changes
45. git diff --staged -- To show staged changes
46. git diff branch1..branch2 -- To compare branches
47. git diff <file> -- To check file differences

===================== REMOTE COMMANDS =====================

48. git remote -v -- To list remotes
49. git remote add origin <url> -- To connect local repo to remote
50. git remote remove origin -- To remove remote
51. git remote rename origin backup -- To rename remote

===================== TAGS (RELEASES) =====================

52. git tag -- To list tags
53. git tag v1.0 -- To create lightweight tag
54. git tag -a v1.0 -m "Release" -- To create annotated tag
55. git push origin v1.0 -- To push tag
56. git push origin --tags -- To push all tags

===================== RECOVERY & CLEANUP =====================

57. git reflog -- To recover deleted commits (life saver)
58. git clean -n -- To preview deletion of untracked files
59. git clean -f -- To delete untracked files
60. git clean -df -- To delete untracked files + folders

===================== FILE / AUTHOR TRACKING =====================

61. git blame <file> -- To see who changed each line
62. git show <commit> -- To show commit details
63. git show HEAD -- To show latest commit details

===================== DEBUGGING =====================

64. git bisect start -- To begin bug search
65. git bisect bad -- To mark commit as bad
66. git bisect good <commit> -- To mark commit as good

===================== CONFIGURATION =====================

67. git config --list -- To list git configurations
68. git config --global user.name "Your Name" -- To set username
69. git config --global user.email "you@email.com" -- To set email
70. git config --global core.editor vim -- To set git editor

===================== SUBMODULE =====================

71. git submodule add <repo> -- To add repo inside repo
72. git submodule update --init -- To initialize submodule

===================== GIT LFS (BIG FILE HANDLING) =====================

73. git lfs install -- To enable large file storage
74. git lfs track "*.zip" -- To track large files
75. git add .gitattributes -- To save tracking rule

===================== IMPORTANT THEORY (INTERVIEW) =====================

Pull vs Fetch vs Rebase vs Merge
git fetch -- downloads changes only
git pull -- fetch + merge
git pull --rebase -- fetch + rebase
git merge -- safe combine
git rebase -- history rewrite

Reset vs Revert
git reset -- undo locally modifies history
git revert -- undo safely keeps history

===================== WHAT DEVOPS MUST KNOW =====================
✔ Pull vs Fetch vs Rebase
✔ Reset vs Revert
✔ Merge conflicts handling
✔ Stash usage
✔ Branch strategy (Dev → QA → Prod)
✔ Tags for releases
✔ Reflog recovery

================================================================================
