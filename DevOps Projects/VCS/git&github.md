# 🔧 Git & GitHub Interview Questions and Answers

---

# 🔹 BASIC VERSION CONTROL QUESTIONS

## 1. What is Version Control?
Version control is a system that tracks changes in code over time.

👉 It helps:
- Collaborate with teams
- Track history
- Restore previous versions

---

## 2. What are types of Version Control Systems?
- Centralized (SVN)
- Distributed (Git)

---

## 3. What is Git?
Git is a distributed version control system used to track changes in code.

---

## 4. What is GitHub?
GitHub is a cloud platform to host Git repositories and collaborate.

---

## 5. Difference between Git and GitHub?
- Git = tool (local)
- GitHub = platform (remote)

---

## 6. What is a repository?
A repository is a folder that contains your project and its version history.

---

## 7. What is a commit?
A commit is a snapshot of your changes.

---

## 8. What is staging area?
The staging area is where changes are prepared before committing.

---

## 9. What is a branch?
A branch is a separate version of code for development.

---

## 10. What is main/master branch?
The main branch is the primary production-ready branch.

---

# 🔹 GIT COMMAND QUESTIONS

## 11. How to initialize a repository?
git init

---

## 12. How to clone a repository?
git clone <url>

---

## 13. How to check status?
git status

---

## 14. How to add files?
git add file
git add .

---

## 15. How to commit changes?
git commit -m "message"

---

## 16. How to view logs?
git log --oneline

---

## 17. How to create a branch?
git branch branch-name

---

## 18. How to switch branch?
git checkout branch-name
git switch branch-name

---

## 19. How to merge branches?
git merge branch-name

---

## 20. How to delete branch?
git branch -d branch-name

---

# 🔹 INTERMEDIATE GIT QUESTIONS

## 21. What is merge conflict?
When two changes affect same file and Git cannot auto-merge.

---

## 22. What is git pull?
Fetch + merge changes from remote.

---

## 23. What is git push?
Upload local commits to remote.

---

## 24. What is git fetch?
Download changes without merging.

---

## 25. What is git rebase?
Reapply commits on top of another branch.

👉 Used for cleaner history

---

## 26. Difference between merge and rebase?
- Merge → keeps history
- Rebase → cleaner history

---

## 27. What is HEAD?
Pointer to current branch/commit.

---

## 28. What is .gitignore?
File to ignore unnecessary files.

---

## 29. What is tagging?
Marking a specific version (e.g., release v1.0)

---

## 30. What is stash?
Temporarily save changes without committing.

---

# 🔹 ADVANCED GIT QUESTIONS

## 31. What is cherry-pick?
Apply specific commit from another branch.

---

## 32. What is revert vs reset?
- revert → creates new commit
- reset → removes commits

---

## 33. What is detached HEAD?
When HEAD is not pointing to a branch.

---

## 34. What is submodule?
A repo inside another repo.

---

## 35. What is shallow clone?
Cloning limited history.

---

## 36. What is reflog?
History of HEAD changes.

---

## 37. What is bisect?
Find bug using binary search.

---

## 38. What is hooks in Git?
Scripts triggered by Git events.

---

## 39. What is fast-forward merge?
Simple merge without extra commit.

---

## 40. What is upstream branch?
Tracking branch for push/pull.

---

# 🔹 GITHUB QUESTIONS

## 41. What is a Pull Request (PR)?
Request to merge code into another branch.

---

## 42. What is fork?
Copy of another repository.

---

## 43. What is GitHub Actions?
CI/CD tool in GitHub.

---

## 44. What is Issues in GitHub?
Used to track bugs and tasks.

---

## 45. What is GitHub Pages?
Host static websites.

---

## 46. What is collaboration workflow?
- Fork → Clone → PR → Merge

---

## 47. What is protected branch?
Branch with restrictions (no direct push).

---

## 48. What is code review?
Review changes before merging.

---

## 49. What is GitHub workflow?
Automation using YAML (CI/CD).

---

## 50. What is release in GitHub?
Packaged version of project.

---

# 🧪 SCENARIO QUESTIONS

## 51. You made mistake in last commit?
git commit --amend

---

## 52. You want to undo changes?
git checkout file

---

## 53. You pushed wrong code?
git revert commit-id

---

## 54. Merge conflict occurred?
- Open file
- Fix manually
- git add
- git commit

---

## 55. Lost changes?
git reflog

---

## 56. Want to save work temporarily?
git stash

---

## 57. Branch not updated?
git pull origin branch

---

## 58. Delete remote branch?
git push origin --delete branch

---

## 59. Sync fork with original repo?
git fetch upstream
git merge upstream/main

---

## 60. Clean repo history?
git rebase -i

---

# 🎯 BEST PRACTICES

- Commit frequently
- Use meaningful messages
- Use branches for features
- Avoid pushing directly to main
- Use pull requests

---
