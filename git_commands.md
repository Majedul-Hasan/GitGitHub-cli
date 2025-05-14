
# Git Commands

## Navigate to a specific drive/folder
```bash
cd :D
```
- This command changes the current directory to the `D` drive on Windows. Replace `D` with any valid drive letter.

## Show all files and folders
```bash
ls
```
- The `ls` command lists all the files and directories in the current directory, but it doesn't include hidden files or directories.

## Show all files and folders, including hidden ones
```bash
ls -a
```
- `ls -a` lists all files and directories, including hidden ones (those starting with a dot, like `.git`).

## Create a new file
```bash
touch <fileName>
```
- `touch` is used to create an empty file with the specified name. For example, `touch readme.md` creates an empty `readme.md` file.

## Git CLI commands

### Check Git config list
```bash
git config --list
```
- This shows all the Git configuration settings for your current repository or user.

### Check the status of the repository
```bash
git status
```
- This shows the current status of the repository, including changes that are staged, unstaged, or untracked.

### Stage all changes
```bash
git add --all
```
- This stages all modified and deleted files for commit.

### Show commit history
```bash
git log
```
- Displays the commit history in the repository, including the commit ID, author, date, and commit message.

### Edit a file (e.g., `readme.md`)
```bash
vi readme.md
```
- Opens the `readme.md` file in the Vim text editor. To save and exit Vim:
```bash
:wq
```

### Show a condensed commit history
```bash
git log --oneline
```
- Displays each commit in a single line, showing the commit ID and the commit message.

### Reset to a specific commit
```bash
git reset --hard <commitId>
```
- Resets the repository to a specific commit ID, discarding any changes after that commit.

### View all commit logs
```bash
git reflog
```
- Displays the history of all Git operations that have changed the branch history (including resets, checkouts, etc.).

### Change to a specific directory
```bash
cd :D
```
- Navigate to the `D` drive or specified directory.

## Branching and Merging

### List all branches
```bash
git branch --list
```
- Lists all branches in the repository.

### Create a new branch
```bash
git branch dev/addheadintext
```
- Creates a new branch called `dev/addheadintext`.

### Switch to a branch
```bash
git switch dev/addheadintext
```
- Switches to the `dev/addheadintext` branch. (You can also use `git checkout dev/addheadintext` in older versions of Git.)

### Merge a branch
```bash
git merge dev/addheadintext
```
- Merges changes from `dev/addheadintext` into the current branch.

## Branch Deletion

### Delete a branch
```bash
git branch -d dev/addheadintext
```
- Deletes the local branch `dev/addheadintext`.

## Rename a branch
```bash
git branch -m dev/addh
```
- Renames the current branch to `dev/addh`.

## Stashing

### Stash changes
```bash
git stash
```
- Stashes any uncommitted changes, saving them temporarily.

### View the list of stashes
```bash
git stash list
```
- Lists all stashes that have been created.

### Apply the most recent stash
```bash
git stash pop
```
- Applies the most recent stash and removes it from the stash list.

### Apply a specific stash
```bash
git stash apply <stashID>
```
- Applies a specific stash using its ID (e.g., `git stash apply stash@{0}`).
