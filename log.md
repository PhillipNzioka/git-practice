## Git Practice

### DAY 1 

Setting up my git, my username and email.

```
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

git config --list

![git config list](<screenshots/day 1 - git config --list.png>)

### DAY 2 First Commit

```
$ git log
commit 3dfa5a783b14593e1719f58c6aafdac18d143088 (HEAD -> main)
Author: PhillipNzioka <nziopindei@gmail.com>
Date:   Sun Jul 12 18:22:51 2026 +0300
```

![git log](<screenshots/day 2 - git log.png>)

### DAY 3 Building the commit habbit

Making three seperate commits today.

![git log oneline](<screenshots/day 3 - git log --oneline.png>)

### DAY 4 .gitignore

Creating a `.gitignore` file in my repsitory and listing files and folders that git won't track into it.

Contents of my .gitignore file
```
# Ignore specific file
secrets.txt

# Ignore all log files
*.log

# Ignore folder and contents
node_modules/ 
screenshots/ 

```

![gitignore](<screenshots/day 4 - .gitignore.png>)

### DAY 5 Branching

Create new branch "feature-1"

`git branch feature-1`

Switch to the new branch 

`git checkout feature-1`

### DAY 6 Merge & Conflict

Merging the new branch `feature-1` to main

![merge branches](<screenshots/Day 6 - merge.png>)

This results in a conflict that I manually resolve to keep the right one by removing the markers
, then I `git add`, followed by `git commit`

![conflict](<screenshots/Day 6 - conflict.png>)

### DAY 7  Checkpoint - Self Test
1. Without looking anything up, write 2–3 sentences answering each question in your log:
2.  What's the difference between git add and git commit?
3. What does a branch actually point to?
4.  What causes a merge conflict?
5. Then look up the real answers and correct yourself where needed.

#### My Answers 
`git add` is git bash command that looks for untracked files or folders in your repository and
stages them (tracks them) ready to be committed.

`git commit` is a git bash command that saves your changes at any given point and allows you to keep record 
of your changes, allowing you to rollback to the correct snapshot of your work. 
It is a snapshot of your file/folder/project at a given time.

A `git branch` points to a copy of my project.

A merge conflict is caused by difference in changes betweern your main and branches that you are merging.

#### Real Answers
The `git add` command moves changes from your working directory to the staging area (index), preparing them for the next commit.  By default, Git does not automatically track changes; you must explicitly use `git add` to specify which files or modifications should be included in your next snapshot.

`git commit` creates a snapshot of your repository’s staged changes, recording the state of the project at a specific point in time along with metadata such as the author, timestamp, and a descriptive message. 

A `git branch` is a lightweight, movable pointer to a specific commit in a repository’s history.  It does not contain or copy the codebase; instead, it simply references the "tip" of a line of development, allowing Git to track the latest state of changes on that branch. As new commits are made, the branch pointer automatically advances to the newest commit, maintaining a continuous chain of project history.

Merge conflicts occur when Git cannot automatically combine changes from different branches because the modifications overlap in ways the system cannot resolve.  This typically happens when two or more developers (or the same developer on different branches) make competing changes to the same lines or regions within the same file. 

### DAY 8 GitHub Setup
Create a GitHub account if you don't have one.
Create a new public repository named git-practice (do not initialize it with a README).
Connect your local repository to the remote one you created on GitHub using the command below.

`git remote add origin <your-repo-url>`

Type the command `git remote -v` in your git terminal and if you get results similar to the one below, then you're successful.

![GitHub Setup](<screenshots/day 8 - github setup.png>)

