### Git Bash

Here are the Git bash instructions.

I've included everything more as a reminder for me if I ever need to use Git on Windows.
Anything after a $ means type on the Git command line

1. In windows explorer navigate to the folder to start the Git repo
2. Right-click and click open Git bash here
3. Click into the Git bash window
4. $ git init

this will start the Git repo in the folder
when you are ready to commit changes to the repo

5. $ git status

the first time you do this in a repo everything will appear as untracked files

6. $ git add --all

this makes Git aware of any untracked files
using a .gitignore file allows you to indicate files that should never be tracked
using git status again should show everything as added files

7. $ git commit -m "<insert commit message>"

this now commits your changes to the repo

8. $ git log

this will show your timestamped commit history and messages
running git status now should say your branch is up to date

continue updating your code until you want to commit again

9. $ git status

[this will tell you modified, deleted and untracked files since the last commit]
[to stage the changes you want added run 10 or 11

10. $ git add <filenames>
11. $ git add --all

because I use .gitignore files to exclude the files I don't want tracking I tend to run git add --all most of the time

11. git commit -m "<insert commit message>"
12. git log
13. git status

[repeat ad infinitum]
