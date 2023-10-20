### Git Setup

```sh
# Set your name for commit markers
git config --global user.name "Your Name"

# Set your email for commit markers
git config --global user.email "your_email@example.com"
```

### Starting a Git Repository

```sh
# Initialize a new git repo in the current directory

git init
# Clone a repository into a new directory

git clone <repo>
```

### Local Changes

```sh
# Check the status of changes as untracked, modified, or staged

git status
# Stage a file to be committed

git add <file>
# Stage all changes to be committed

git add .
# Commit the staged snapshot, but instead of launching a text editor, use the given message

git commit -m "Commit message"
# Commit all local changes in tracked files

git commit -a
# Show diff of files that are not yet staged

git diff
# Show diff of files that are staged but not yet committed

git diff --staged
```

### Change History

```sh
# Show entire commit history

git log
# Show history in a compact format

git log --oneline
# Show changes over time for a specific file

git log -p <file>
```

### Branches & Tags

```sh
# List all local branches in the repository

git branch
# Create a new branch

git branch <branch>
# Switch to a branch

git checkout <branch>
# Create and switch to a new branch

git checkout -b <branch>
# Merge a different branch into your active branch

git merge <branch>
# Create a tag at the current commit

git tag <tag_name>
```

### Update & Publish

```sh
# List all currently configured remotes

git remote -v
# Add a new remote repository

git remote add <name> <url>
# Download all changes from <remote>, but don't integrate into HEAD

git fetch
# Download changes and directly merge/integrate into HEAD

git pull
# Publish local changes on a remote

git push <remote> <branch>
# Push tags to remote repository

git push --tags
```

### Merge & Rebase

```sh
# Merge <branch> into your current HEAD

git merge <branch>
# Reapply commits on top of another base tip

git rebase <branch>
# Abort a rebase

git rebase --abort
# Continue a rebase after resolving conflicts

git rebase --continue
```

### Undo

```sh
# Create a new commit that undoes all of the changes made in <commit>, then apply it to the current branch

git revert <commit>
# Reset your HEAD pointer to the latest commit and discard all changes in the working directory and staging area

git reset --hard HEAD
# Reset your HEAD pointer to a previous commit and discard all changes since then

git reset --hard <commit>
```

### Collaborating

```sh
# Fetch down all the branches from that Git remote

git fetch <remote>
# Merge a remote branch into your current branch to bring it up to date

git merge <remote>/<branch>
# Transmit local branch commits to the remote repository branch

git push <remote> <branch>
# Fetch and merge any commits from the tracking remote branch

git pull
```

### Stashing

```sh
# Stash your changes

git stash
# Re-apply your stashed changes

git stash pop
# List all stashed changesets

git stash list
# Discard the most recently stashed changeset

git stash drop
```
