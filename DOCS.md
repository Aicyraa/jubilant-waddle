Note: Always use git commit --ammend or reset when editing previous commits

HEAD points to a branch
HEAD~2 means 2 commit prior to the current commit

git commit --amend
   * allows us to edit the last commit (replace entirely)
   * We can use this when we forgot to add a file during commit

git rebase -i HEAD~2 ; 2 means 2 previous commits
   * Allows us to edit multiple commits
   * It will bring you first to your code editor text editor -> then you can modify the option for each commit like edit, pick, squash -> Then it will bring you back from commit where you specify "edit" to the latet ongoing change
   
squashing 
   * Allows us to combine or merge commits

git reset HEAD~
   * Resets the commit, unstaging the stage file

git reset --soft HEAD~
   * Resets the commit prior to the current commit and staged files is still staged

HEAD 
   * HEAD -> Branch -> Latest Commit

Detached HEAD
   * WHen you checked out a commit with its id
   * You can edit and commit while in a detached state and bracnes will not be affected. If you want to save the commited file, you may create a new branch

Process (If you wnat to change files)
   * Rebase -> You will be pointed at the commit after your target commit -> Make changes then stage it -> amend then update the commit message -> continue
   * There is times that ur changed will get a conflict. Open the conflict -> solve the conflict -> stage -> continue
