Reset

Sunday, January 29, 2023

12:21 PM

 

git reset

Reset staging area to match most recent commit, but leave the working directory unchanged.

 

git reset \--hard

Reset staging area and working directory to match most recent commit and overwrites all changes in the working directory.

 

git reset \<commit\>

Move the current branch tip backward to \<commit\>, reset the staging area to match, but leave the working directory alone.

 

git reset \--hard \<commit\>

Same as previous, but resets both the staging area & working directory to match. Deletes uncommitted changes, and all commits after \<commit\>.
