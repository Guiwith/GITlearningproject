# Git Command Learning Guide

## Basic Operations
```bash
# Initialize repository
git init 

# Add files to staging area
git add .

# Commit changes
git commit -m "your title"

# Add remote repository
git remote add origin YOURGITRES

# Set main branch name
git branch -M main

# Push to remote repository (you can use -u to track your branch)
git push -u origin main

# Then you can update like THIS
git add .
git commit -m "TITLE"
git push
```

## Proxy Settings
```bash
# If your IDE outputs a 433 error or cannot connect to GitHub
# TRY THIS COMMAND (this will change proxy to your VPN)
git config --global http.proxy http://127.0.0.1:7890
git config --global https.proxy http://127.0.0.1:7890
```

## Branch Operations
```bash
# Make a branch
git checkout -b BRANCHNAME

# Switch to branch
git branch
git switch BRANCHNAME

# Merge a Branch (you have to switch to main branch first)
git checkout main
git merge BRANCHNAME

# Delete branch
git branch -d BRANCHNAME    # LOCAL
git push origin --delete BRANCHNAME    # REMOTE
```

## Version Control
```bash
# Check update log
git log

# Drop not added changes
git restore .

# Get back to old version
git reset --hard ID
```

## Stash Operations
```bash
# Stash (you can store your unfinished branch here)
git stash list 
git stash

# Back to your job
git stash pop    # This will delete stash
git stash apply  # This will not delete stash

# Or delete it
git stash drop
```

## Rebase Operations
```bash
# Rebase (make your push as one line, DO NOT USE IT IN TEAM WORK)
git rebase main
```