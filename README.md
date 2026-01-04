# hello-world

# 1. Fetch latest refs
git fetch origin

# 2. Define release no
RELEASE_NUMBER=204

# 3. Create release branch from main
git checkout -b release/$RELEASE_NUMBER  origin/main

# 4. Merge develop into release/203
git merge origin/develop

# 5. Resolve conflicts if any, then commit (only if Git asks)
# git add .
# git commit

# 6. Push release branch to GitHub
git push -u origin release/$RELEASE_NUMBER 
