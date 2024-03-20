# Git Commands Guide

## Repository Setup

- `git init`: Initialize a new Git repository
- `git clone <repository_url>`: Clone an existing repository from a remote URL
- `git config --global user.name "<your_name>"`: Set your global Git username
- `git config --global user.email "<your_email@example.com>"`: Set your global Git email address

## Basic Workflow

- `git add <file_name>`: Add a file to the staging area
- `git commit -m "Commit message"`: Commit changes to the local repository
- `git status`: Check the status of files in the working directory
- `git diff`: Show changes between commits, commit and working tree, etc.

## Branching and Merging

- `git branch`: List all branches in the repository
- `git branch <branch_name>`: Create a new branch
- `git checkout <branch_name>`: Switch to a different branch
- `git merge <branch_name>`: Merge changes from a different branch into the current branch

## Remote Repositories

- `git remote add <remote_name> <remote_url>`: Add a new remote repository
- `git push <remote_name> <branch_name>`: Push changes to a remote repository
- `git pull <remote_name> <branch_name>`: Pull changes from a remote repository

## Undoing Changes

- `git reset <file_name>`: Unstage changes for a file
- `git checkout -- <file_name>`: Discard changes in the working directory for a file
- `git revert <commit_id>`: Revert a commit and create a new commit with the reverted changes
- `git reset --hard <commit_id>`: Reset the current branch to a specific commit and discard all changes

## History and Logging

- `git log`: View commit history
- `git log --oneline`: View condensed commit history
- `git blame <file_name>`: Show who last modified each line of a file
