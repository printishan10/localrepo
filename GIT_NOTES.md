📘 GIT & GITHUB COMPLETE NOTES (Beginner → Strong Base)
🧠 1. What is Git?
Git = Version Control System (VCS)
Tracks changes in code over time
Lets you:
Go back to previous versions
Work in teams
Manage projects efficiently
🌐 2. What is GitHub?
GitHub = Cloud platform for Git repositories
Used to:
Store code online
Collaborate with others
Share projects
⚙️ 3. Git Setup (First Time)
git config --global user.name "Your Name"
git config --global user.email "your@email.com"

Check config:

git config --list
📁 4. Initialize Repository
git init

👉 Creates hidden .git folder → makes it a Git repo

📌 5. Git Workflow (MOST IMPORTANT)
Working Directory → Staging Area → Repository
Commands:
git add filename
git add .
git commit -m "message"
🔍 6. Check Status
git status

Shows:

Modified files
Staged files
Untracked files
📊 7. Git Log
git log

👉 Shows commit history

Short version:

git log --oneline
🆕 8. Add & Commit
Add:
git add .
Commit:
git commit -m "Your message"
🔄 9. Modify & Track Changes

After editing:

git status
git diff

👉 git diff shows exact changes

🚫 10. .gitignore

Used to ignore files (like):

node_modules
.env
temp files

Create file:

.gitignore

Example:

node_modules/
.env
🔗 11. Connect to GitHub
git remote add origin <repo-link>

Check:

git remote -v
⬆️ 12. Push Code to GitHub
git push origin main

First time:

git push -u origin main
⬇️ 13. Pull Code from GitHub
git pull origin main

👉 Gets latest code from GitHub

🌿 14. Branching (VERY IMPORTANT)
Create branch:
git branch feature1
Switch branch:
git checkout feature1

OR:

git checkout -b feature1
📍 15. Check Branches
git branch

👉 * shows current branch

🔀 16. Merge Branch

Switch to main:

git checkout main

Merge:

git merge feature1
❌ 17. Delete Branch
git branch -d feature1
⚔️ 18. Merge Conflicts (Important)

Happens when:

Same file edited in 2 branches

Fix:

Open file
Remove conflict markers:
<<<<<<< HEAD
=======
>>>>>>> feature1
Edit manually
Then:
git add .
git commit
🔄 19. Fork (GitHub Concept)
Copy someone else's repo to your GitHub
Used for:
Open source contributions
🔁 20. Clone Repository
git clone <repo-link>
🔄 21. Undo Changes (Basic)
Before adding:
git restore filename
After adding:
git restore --staged filename
🧩 22. Important Commands Summary
git init
git status
git add .
git commit -m "msg"
git log --oneline
git branch
git checkout branch_name
git merge branch_name
git push origin main
git pull origin main
⚡ 23. Key Concepts to Remember
Git works inside a folder (.git)
Always SAVE → ADD → COMMIT
GitHub ≠ Local repo (you must push/pull)
Branching = safe experimentation
Pull before push (avoid conflicts)
🧠 24. Mental Model (VERY IMPORTANT)

Think like this:

👉 Git = your local history tracker
👉 GitHub = your online backup + collaboration tool