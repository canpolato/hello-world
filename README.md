# hello-world

## Release Branch Creation
### 1. Fetch latest refs
git fetch origin

### 2. Define release no
RELEASE_NUMBER=204

### 3. Create release branch from main
git checkout -b release/$RELEASE_NUMBER  origin/main

### 4. Merge develop into release/203
git merge origin/develop

### 5. Resolve conflicts if any, then commit (only if Git asks)
git add .
git commit

### 6. Push release branch to GitHub
git push -u origin release/$RELEASE_NUMBER 

-------------

## Feature Branch Creation
### 1. Fetch latest refs
git fetch origin

### 2. Define feature branch name
FEATURE_NAME=302

### 3. Create feature branch from develop
git checkout -b feature/$FEATURE_NAME  origin/develop

### 4. Resolve conflicts if any, then commit (only if Git asks)
git add .
git commit -m "test"

### 6. Push feature branch to GitHub
git push -u origin feature/$FEATURE_NAME 
