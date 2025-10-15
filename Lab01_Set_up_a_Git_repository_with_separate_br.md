# Lab 01: Set up a Git repository with separate branches for frontend and backend, then merge them into the main branch.

## Objective
To create a Git repository with separate branches for frontend and backend development, and merge both branches into the main branch.  
This demonstrates basic Git operations and branch management.

## Tools / Technologies
-Git  
- GitHub  
- VS Code or GitHub Codespaces  
- Command Line / Terminal  


## Prerequisites
- Git installed on your system  
- A GitHub account  
- Basic understanding of Git commands  
- Repository already created using GitHub Classroom  


## Steps / Commands
Step 1 — Initialize a Git repository
bash
git init 
git checkout -b frontend
echo "<h1>Frontend</h1>" > index.html
git add index.html
git commit -m "Added frontend code"
git checkout main
git checkout -b backend
echo "print('Backend running')" > app.py
git add app.py
git commit -m "Added backend code"
git checkout main
git merge frontend
git merge backend
git remote add origin https://github.com/sravyareddy-29/insem_1_sravya
git push -u origin main

## Expected Output / Result
A GitHub repository (e.g., insem_1_sravya) with:
Three branches:
main
frontend
backend

Merged Code in Main Branch:
index.html (from the frontend branch)
app.py (from the backend branch)

## Deliverables (what to push)
- `Labs/Lab01_<ShortTitle>.md` (this file, completed)
- Any additional scripts, Dockerfiles, manifests, or screenshots placed in a folder named `Lab01_files/`

## Notes / Tips
Use git status often to verify which branch you are on and which files are staged or committed.

