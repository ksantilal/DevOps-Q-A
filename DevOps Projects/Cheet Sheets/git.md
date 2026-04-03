# Git Cheat Sheet

## ⚙️ Setup
- `git config --global user.name "Name"` → Set username
- `git config --global user.email "email"` → Set email

## 📦 Repository
- `git init` → Initialize repo
- `git clone <url>` → Clone remote repo

## 📌 Staging
- `git add .` → Add all changes
- `git add file` → Add specific file

## 💾 Commit
- `git commit -m "message"` → Save snapshot

## 🌿 Branching
- `git branch` → List branches
- `git checkout -b branch` → Create + switch branch
- `git switch branch` → Switch branch

## 🔀 Merge
- `git merge branch` → Merge into current branch

## ☁️ Remote
- `git remote add origin url` → Add remote repo
- `git push -u origin main` → Push code
- `git pull` → Fetch + merge updates

## 📜 Logs
- `git log --oneline` → Compact history
- `git status` → Current changes

- `git remote remove origin` -> remove old remote repo
- `git remote remove origin your repo` -> add new repo 
- `git remote -v`-> verify repo


- git branch -m feature1 feature-1 -> to rename branch
- git branch -d feature1 -> remove the branch
