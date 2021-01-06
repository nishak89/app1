# app1
This is a Tutorial 

Undoing Things:
==============
git clean
   undoing uncommitted changes
   $ git clean -n //dry run
   $ git clean -f //force clean
   $ git clean -d //remove untracked directories

git checkout
   commit level   - Switch between branches or use it view an old revision
   file level     - discard changes in the working directory
   $ git checkout commit
   $ git checkout branch

git reset
   commit level   - throw away uncommitted changes or discard commits in a private branch
   file level     - unstage a file
   $ git reset --hard commit
   $ git reset file // to unstage file after adding it using git add 

git revert
   commit level   - undo commits in public branch
   $ git revert HEAD

Summary:
1. Use "git checkout" to move around and review the commit history
2. "git revert" is the best tool for undoing shared public changes
3. "git reset" is best used for undoing local private changes


