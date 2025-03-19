# Task 3 - Version Control Operations


## Steps Performed

### 1️⃣ Creating and Tracking Files
- Created sample files:
  - `task-03/File1.txt`
  - `task-03/File2.txt`
- Checked repository status:
 
  git status

   Verified that the new files were untracked.

- Added files for tracking:

  git add .

- Committed the changes:
   
  git commit -m "Created sample files for executing task 3"
   
- Pushed changes to the remote repository:
   
  git push origin main
   

 

### 2️⃣ Modifying Files and Managing Changes
- Modified `File1.txt` and `File2.txt`.
- Checked the status:
   
  git status
   
  - Confirmed changes in both files.

- Restored `File1.txt` to the last committed version:
   
  git restore task-03/File1.txt
   

- Staged and committed the updated files:
   
  git add .
  git commit -m "two files are staged"
   

 

### 3️⃣ Reverting Changes and Fixing Errors
- Attempted to restore a file directly:
   
  git restore File1.txt
   
  - **Error:** The file was not recognized in the tracked state.

- Checked repository status:
   
  git status
   
  - **Git Warning:** CRLF will replace LF in `File2.txt` during the next update.

- Attempted to revert the last commit:
   
  git revert HEAD
   
  - **Error:** Local changes would be overwritten by revert.

- Committed the current changes before reverting:
   
  git commit -m "current changes before reverting"
   

- Successfully reverted the last commit:
   
  git revert HEAD
   

 

### 4️⃣ Final Status Check and Push
- Verified the repository status:
   
  git status
   
  - **Result:** The branch was ahead by three commits.

- Staged all changes:
   
  git add .
   

- The repository is now in sync with the required changes.

 

