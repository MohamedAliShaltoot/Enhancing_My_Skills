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

### How to Add Some Style to Your Notes (CSS)
If you're using this `README.md` on a personal website or custom project, you can enhance its look by adding some **CSS** for hover effects, like:

```html
<style>
  h3 {
    font-size: 1.2em;
    color: #4CAF50;
    transition: all 0.3s ease;
  }

  h3:hover {
    color: #FF5733;
    cursor: pointer;
  }

  code {
    background-color: #f4f4f4;
    border-radius: 5px;
    padding: 0.3em;
  }

  .note {
    background-color: #f9f9f9;
    padding: 10px;
    border-radius: 8px;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
    margin-bottom: 15px;
    transition: background-color 0.3s ease;
  }

  .note:hover {
    background-color: #e0f7fa;
  }
</style>
