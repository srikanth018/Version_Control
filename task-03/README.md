# Task 3 - Version Control Operations


## Steps Performed

### 1️⃣ Creating and Tracking Files
- Created sample files:
  - `task-03/File1.txt`
  - `task-03/File2.txt`
- Checked repository status:
  ```sh
  git status
  ```
  - Verified that the new files were untracked.

- Added files for tracking:
  ```sh
  git add .
  ```
- Committed the changes:
  ```sh
  git commit -m "Created sample files for executing task 3"
  ```
- Pushed changes to the remote repository:
  ```sh
  git push origin main
  ```

---

### 2️⃣ Modifying Files and Managing Changes
- Modified `File1.txt` and `File2.txt`.
- Checked the status:
  ```sh
  git status
  ```
  - Confirmed changes in both files.

- Restored `File1.txt` to the last committed version:
  ```sh
  git restore task-03/File1.txt
  ```

- Staged and committed the updated files:
  ```sh
  git add .
  git commit -m "two files are staged"
  ```

---

### 3️⃣ Reverting Changes and Fixing Errors
- Attempted to restore a file directly:
  ```sh
  git restore File1.txt
  ```
  - **Error:** The file was not recognized in the tracked state.

- Checked repository status:
  ```sh
  git status
  ```
  - **Git Warning:** CRLF will replace LF in `File2.txt` during the next update.

- Attempted to revert the last commit:
  ```sh
  git revert HEAD
  ```
  - **Error:** Local changes would be overwritten by revert.

- Committed the current changes before reverting:
  ```sh
  git commit -m "current changes before reverting"
  ```

- Successfully reverted the last commit:
  ```sh
  git revert HEAD
  ```

---

### 4️⃣ Final Status Check and Push
- Verified the repository status:
  ```sh
  git status
  ```
  - **Result:** The branch was ahead by three commits.

- Staged all changes:
  ```sh
  git add .
  ```

- The repository is now in sync with the required changes.

---

