## This is for git command learning
git init 
git add .
git commit -m "your title"
git remote add origin YOURGITRES
git branch -M main
git push -u origin main
# Then u can update like THIS
git add .
git commit -m "TITLE"
git push
# If your ide output a 433 erro or can not connect to github 
# TRY THIS COMMAND(this will change proxy to your VPN)
git config --global http.proxy http://127.0.0.1:7890
git config --global https.proxy http://127.0.0.1:7890
# Make a branch
git checkout -b BRANCHNAME
# Switch to branch
git branch
git switch BRANCHNAME
# Merge a Branch(you have to switch to main branch first)
git checkout main
git merge BRANCHNAMR
# Delete branch
git branch -d BRANCHNAME(LOCAL)
git push origin --delete BRANCHNAME(REMOTE)
# Check update log
git log
# Drop not added changes
git restore .
# Get back to old version
git reset --hard ID