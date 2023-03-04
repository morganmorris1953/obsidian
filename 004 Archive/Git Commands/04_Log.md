Log

Sunday, January 29, 2023

12:23 PM

 

git log -\<limit\>

Limit number of commits by \<limit\>.

E.g. "git log -5" will limit to 5 commits

 

git log \--oneline

Condense each commit to a single line

 

git log -p

Display the full diff of each commit.

 

git log \--stat

Include which files were altered and the relative number of

lines that were added or deleted from each of them.

 

git log \--author= "\<pattern\>"

Search for commits by a particular author.

 

git log \--grep="\<pattern\>"

Search for commits with a commit message that matches \<pattern\>

 

git log \<since\>..\<until\>

Show commits that occur between \<since\> and \<until\>. Args can be a

commit ID, branch name, HEAD, or any other kind of revision reference.

 

git log \-- \<file\>

Only display commits that have the specified file.

 

git log \--graph \--decorate

\--graph flag draws a text based graph of commits on left side of commit

messages. \--decorate adds names of branches or tags of commits shown
