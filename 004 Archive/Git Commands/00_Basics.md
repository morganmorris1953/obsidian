Basics

Sunday, January 29, 2023

9:16 AM

 

git init \<directory\>

Create empty Git repo in specified directory. Run with no arguments to initialize the current directory as a git repository

 

Git clone \<repo\>

Clone repo located at onto local machine. Original repo can be located on the local filesystem or on a remote machine via HTTP or SSH.

 

Git config user.name \<name\>

Define author name to be used for all commits in current repo. Devs commonly use \--global flag to set config options for current user

 

Git add \<directory\>

Stage all changes in for the next commit. Replace with a to change a specific file.

 

git commit -m \"\<message\>\"

Commit the staged snapshot, but instead of launching a text editor, use \<message\> as the commit message.

 

Git status

List which files are staged, unstaged, and untracked

 

Git log

Display the entire commit history using the default format. For customization see additional options

 

Git diff

Show unstaged changes between your index and working directory
