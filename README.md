# 📝 Git Notes

## 📌 Common Git Commands & Tips

1. **Create and switch to a new branch:**
   bash
   git checkout -b branchName
   

2. *Add and commit changes in one step:*
   bash
   git commit -am "Your commit message"
   

3. *Unstage a file after using `git add`:*
   bash
   git reset fileName
   

4. *Creating a Pull Request after pushing a commit:*
   - If no "Pull Request & Compare" button appears, look for the *Contribute* dropdown.
   - Click it and you'll find the option to create a pull request.

5. *Delete a branch:*
   - First, switch to another branch.
   - Then run:
     bash
     git branch -d branchName
     

6. *Rebase vs Merge:*
   - *Rebase* rewrites commit history to make it linear and clean.
   - *Merge* combines branches and preserves history, which can result in a more complex graph.
   - To rebase:
     bash
     git rebase targetBranch
     

7. *Ignore a file after it's been added to Git:*
   - First, remove it from tracking (but not from your local folder):
     bash
     git rm --cached lab1.xml library.json
     
   - Then make sure it's listed in `.gitignore`:
     
     lab1.xml
     library.json
     
   - Commit the change:
     bash
     git commit -m "Stop tracking lab1.xml and library.json"
   
