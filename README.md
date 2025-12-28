# Git Workflow Notes

Welcome to the Git tips and tricks guide! Here are some essential commands and concepts to help you streamline your workflow.

---

### 1. Create a New Branch
Use `git checkout -b branchName` to create a new branch and switch to it.

---

### 2. Add and Commit in One Step
Use `git commit -am "message"` to add and commit your changes in one go.

---

### 3. Unstage a File
If you want to unstage a file after using `git add`, run `git reset <fileName>`.

---

### 4. Create a Pull Request Manually
If you pushed a new commit but don’t see the **Pull Request & Compare** button:
- Click the **Contribute** dropdown menu.
- Create a **Pull Request** from there.

---

### 5. Delete a Branch
To delete a branch, follow these steps:
1. First, make sure you are on a different branch.
2. Run `git branch -d branchName`.

---

### 6. Rebase vs Merge
Learn how to use **Rebase** in Git and understand the difference between **Rebase** and **Merge**.

---

### 7. Add a File to `.gitignore`
If you added a file that should be ignored:
1. Run `git rm --cached lab1.xml library.json` to stop tracking the file.
2. Add the file(s) to `.gitignore`.

---

### 8. View Commit Details
To see what a specific commit did, run `git show commit_id`.

---

### 9. Revert a Commit
If you want to remove unwanted changes from a commit, use:
- `git revert commit_ID`.

---

### 10. Stash Your Changes Temporarily
If you need to switch tasks but want to save your current work:
1. Run `git stash` to temporarily save your changes.
2. After finishing the other task, apply the stashed changes using `git stash apply stash@{0}`.

---

### 11. Create and Push a Tag
To create a new tag:
1. Run `git tag tagName commit_ID`.
2. To push your tags to the repository, use `git push --tags`.

---


