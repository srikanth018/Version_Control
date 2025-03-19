# Task 3 - Version Control Operations


## Steps Performed

- Created sample files:
  - `task-03/File1.txt`
  - `task-03/File2.txt`
- Checked repository status:
 
  git status
  
- Added files for tracking:

  git add .

- Committed the changes:
   
  git commit -m "Created sample files for executing task 3"
   
- Pushed changes to the remote repository:
   
  git push origin main
   
- Modified `File1.txt` and `File2.txt`.
- Checked the status:
   
  git status
   
  - Confirmed changes in both files.

- Restored `File1.txt` to the last committed version:
   
  git restore task-03/File1.txt
   

- Staged and committed the updated files:
   
  git add .
  git commit -m "two files are staged"
   

- Checked repository status:
   
  git status
   
  git revert HEAD
   
- Successfully reverted the last commit:
   
  git revert HEAD
   
