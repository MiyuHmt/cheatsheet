# Git

## Git setup

Global setup:

```bash
git config --global user.name "Firstname Lastname"
git config --global user.email "jame.doe@example.com"
```

Local setup:

```bash
git config user.name "Firstname Lastname"
git config user.email "jame.doe@example.com"
```

Set automatic commnand line coloring for Git:
```bash
git config --global color.ui auto
```

## Create

Clone an existing repository:

```bash
git clone <HTTPS or SSH url>
```

Initialize an existing directory as a Git repo:

```bash
git init
```

## Local changes

Changed files in your working directory:
```bash
git status
```

Diff of what is changed but not staged:
```bash
git diff
```

Diff of what is staged but not yet commited:
```bash
git diff --staged
```

Add all current changes to the next commit (stage):
```bash
git add .
```

Add a specific file to the next commit (stage):
```bash
git add <file>
```

Commit staged content with a descriptive message:
```bash
git commit -m "the message"
```

Change the last commit:
```bash
git commit --amend
```

## Commit history

Show all commits:
```bash
git log
```

Show changes over time for a specific file:
git log -p file

## Branches
Lising all branches
```bash
git branch -av
```

Switch branch:
```bash
git checkout <branch>
```

Create a new banch:
```bash
git branch <new-branch>
```

Delete a local branch:
```bash
git branch -d <branch>
```

## Update and publish

Download changes and merge into HEAD:
```bash
git pull <remote> <branch>
```
Publish local changes on a remote:
```bash
git push <remote> <branch>
```

## Merge

Merge branch into the current HEAD:
```bash
git merge <branch>
```

## Undo
Discard all local changes in your working directory:
```bash
git reset -hard HEAD
```

Discard local changes in a specific file:
```bash
git checkout HEAD <file>
```

Revert a commit:
```bash
git revert <commit>
```
Unstage a file while retaining the changes in working directory
```bash
git reset <file>
```
