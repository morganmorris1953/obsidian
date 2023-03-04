Remote Repositories

Sunday, January 29, 2023

9:18 AM

 

git remote add \<name\> \<url\>

Create a new connection to a remote repo. After adding a remote,

you can use \<name\> as a shortcut for \<url\> in other commands.

 

 

git fetch

\<remote\> \<branch\>

Fetches a specific \<branch\>, from the repo. Leave off \<branch\>

to fetch all remote refs.

 

git pull \<remote\>

Fetch the specified remote's copy of current branch and

immediately merge it into the local copy.

 

git push \<remote\> \<branch\>

Push the branch to \<remote\>, along with necessary commits and

objects. Creates named branch in the remote repo if it doesn't exist

 
