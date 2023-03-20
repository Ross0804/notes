## Basic Git Commands

- **git init** initializes a brand new git repository and begins tracking an existing directory.
- **git clone** creates a local copy of a project that already exists remotely.
- **git add** stages a change.
- **git commit** saves the snapshot to the project history and completes the change-tracking process.
- **git status** shows the status of changes as untracked, modified, or staged.
- **git branch** shows the branches being worked on locally.
- **git merge** merges lines of development together, typically merging from a feature branch back to main.
- **git pull** updates the local line of development with updates from its remote counterpart. Typically used to pull commits from another developer from a remote branch, so that the changes are reflected in the local environment.
- **git push** updates the remote repository with any commits made locally to the branch.

## Example: Contribute to an existing repository

```bash
# downlaod a repository on GitHub to our machine
git clone https://github.com/Ross0804/notes.git

# change into the directory
cd notes

# create a new branch to store any new changes
git branch my-branch

# switch to that branch (line of development)
git checkout my-branch

# make your changes

# stage the changed files
git add file1.md file2.md

# take a snapshot of the staging area
git commit -m "my snapshot"

# push changes to remote repo
git push --set-upstream origin my-branch
```