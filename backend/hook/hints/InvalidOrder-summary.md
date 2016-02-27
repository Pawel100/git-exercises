The easiest way to change order of commits in history is to use rebase interactive
feature of Git. Just swap the commits as you want leaving default pick operation.

Remember that you don't need to know the commit SHA-1 hashes when specifying
them in git rebase -i command. When you know that you want to go 2 commits
back, you can always run git rebase -i HEAD^^ or git rebase -i HEAD~2.

Note that you should not change commits order when you have published them already.
Need to know why? See: http://git-scm.com/book/en/v2/Git-Branching-Rebasing#The-Perils-of-Rebasing

For more info, see: http://git-scm.com/book/en/v2/Git-Tools-Rewriting-History#Reordering-Commits