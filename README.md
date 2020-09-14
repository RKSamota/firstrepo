

Hello everone in this repository I am going to tell about basic commends of git with example.


#  1.   git init  : -
This command turns a directory into an empty Git repository. This is the first step in creating a repository. 

Example :-   
make directory a git repository
$ git init


# s2.  git add  :-
Adds files in the to the staging area for Git. Before a file is available to commit to a repository, the file needs to be added to the Git index (staging area).

Example :- 
To stage a specific file:
$ git add index.html

To stage an entire directory:
$ git add mydirectory 

//To add all files not staged:
          $ git add .


#3.  git commit  : -

Record the changes made to the files to a local repository. For easy reference, each commit has a unique ID. 

Example: -
// Adding a commit with message
$ git commit -m "Commit message in quotes"

#4.  git status  : -

git status will return the current working branch. If a file is in the staging area, but not committed, it shows with git status. Or, if there are no changes it’ll return nothing to commit, working directory clean.

Example : -
 Message when files have not been staged (git add)
$ git status
On branch SecretTesting
Untracked files:
  (use "git add <file>..." to include in what will be committed)

  	homepage/index.html

# Message when files have been not been committed (git commit)
$ git status
On branch SecretTesting
Your branch is up-to-date with 'origin/SecretTesting'.
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   homepage/index.html

Message when all files have been staged and committed 
$ git status
On branch SecretTesting
nothing to commit, working directory clean


#5.   git config  :-

It is used for configure the user information like username, useremail and password  etc.

Example:-
$ git config <setting> <command>

Running git config globally
$ git config --global user.email "my@emailaddress.com"
$ git config --global user.name "myusername"

Running git config on the current repository settings
$ git config user.email "my@emailaddress.com"
$ git config user.name "myusername"

