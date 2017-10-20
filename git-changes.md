## Git Commands

### Definitions

untracked files: files which have never been git added
tracked files: file that are being version by git
staging: the action performed by doing a git add (staging the changes for commit)

unstaged changes appear red in git status
staged changes appear green in git status

### Undoing changes before commit

#### Untracked files

To remove untracked file:
```
git clean -f <FILE>
```
To remove all untracked changes:
```
git clean -f .
```

To unstage a new file (turn it back from green to red):
```
git reset HEAD <FILE>
```
Then git clean can be used to remove the file
 
#### Tracked files

To undo changes to a file since the last commit (before you do a git add) (appears red with the word modified):
```
git checkout <FILE>
```
To undo all changes to tracked files
```
git checkout .
```

Again if you have already stageed the changes then first perform the git reset:
```
git reset HEAD <FILE>
```
or to unstage all changes (tracked and untracked files)
```
git reset HEAD
```

