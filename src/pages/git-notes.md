---
layout: ../layouts/MarkdownLayout.astro
---

# Git Notes

## Install Git

Visit [Git-Downloads](https://www.git-scm.com/downloads) to get instructions for installing git.


## Get Git Version

```bash
git --version
```

## Configure Git on Local Machine

```bash
# Set user name.
git config --global user.name "SamSpade"

# Set user email.
git config --global user.email "samspade@test.com"

# Shot config settings.
git config --list
```

If you want to set the user name and email only for a specific repository, remove `global`.

## Initialize Git Repository

```bash
git init
```

## Check the Status of Repository

```bash
# Check the status of your repository.
git status

# Shorthand version.
git status --short
```

Short status flags:

- ?? - Untracked files
- A - Files added to stage
- M - Modified files
- D - Deleted files

## Staging files

```bash
# Stage a file by name.
git add <filename>

# Stage multiple files.
git add --all | .
```

## Commiting staged file

```bash
git commit -m "message"

# Stage all changed and tracked files.
git commit -a -m "message"
```

## See the history of commits

```bash
git log

# Show one line at a time.
git log --oneline
```

**Note**: If there is a long list view in the terminal, `shift + G` to jump to the end of the list, then `q` to exit the list.

## Git Branches

```bash
# Create a new branch.
git branch branch_name

# Checkout a branch.
git checkout branch_name

# Create a new branch and move to it immediately.
git checkout -b branch_name

# List all branches in repository.
git branch

# Merge branches.
git merge branch_name

# Delete a branch
git branch -d branch_name

# Force delete a branch.
git branch -D branch_name
```


## Working with GitHub

Create a repository on GitHub.
Copy the URL of the repository and use that URL to set the origin in our local repo.

```bash
git remote add origin github_repo_url
```

Now we can push our master branch to the origin url, and set it as the default remote branch.

```bash
git push --set-upstream origin master

# Shorthand command.
git push -u origin master
```

To see which remote servers we have configured:

```bash
git remote

# List all the remote repositories connected to our local repository.
git remote -v

# Set a new url for origin.
git remote set-url origin <new-url>
```

## Git Pull

Git ```pull``` is a combination of ```fetch``` and ```merge```. It pulls all the changes from a remote repository into the branch of a local one.

```bash
git pull origin
```

## Git Push

```bash
git push origin
```

## Git Clone

```bash
git clone github_repo_url
```