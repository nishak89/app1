This is a GIT Tutorial 

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

Git patching:
============
To create patch
   1. git diff > name-of-file.patch
   2. git format-patch -n <commit>
   3. git show <commit> > name-of-file.patch

To apply patch
   1. git apply name-of-file.patch
   2. patch -p1 < name-of-file.patch
   3. git am name-of-file.patch

