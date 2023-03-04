Config

Sunday, January 29, 2023

12:15 PM

 

git config \--global user.name \<name\>

Define the author name to be used for all commits by the current user.

 

git config \--global user.email \<email\>

Define the author email to be used for all commits by the current user.

 

git config \--global alias. \<alias-name\> \<git-command\>

Create shortcut for a Git command. E.g. alias.glog "log \--graph \--oneline" will set "git glog" equivalent to "git log \--graph \--oneline.

 

git config \--system core.editor \<editor\>

Set text editor used by commands for all users on the machine. \<editor\>

arg should be the command that launches the desired editor (e.g., vi).

 

Git config \--global \--edit

Open the global configuration file in a text editor for manual editing.
