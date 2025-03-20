# Task 4: Simulating and Resolving Merge Conflicts


## Steps Followed

### 1. **Create Two Branches**
We first create two branches, `test1` and `test2`, from the current working branch.

### 2. **Switch to `test1` and Make Changes**
- Switch to branch `test1`, make changes to the `ProgrammingLanuages.txt` file, and commit them.



Modify `ProgrammingLanuages.txt` by adding:

```
Programming languages:
- Java
- Python
- Ruby  ---->Changes Made
- JavaScript  ---->Changes Made
```

Add and commit the changes


### 3. **Switch to `test2` and Make Different Changes**
- Switch to `test2`, make different changes to the same file, and commit them.

Modify `ProgrammingLanuages.txt` by adding:

```
Programming languages:
- Java
- Python
- PHP   ---->Changes Made
- C/C++  ---->Changes Made
```

Add and commit the changes to same file



### 4. **Merge `test2` into `test1` (Conflict Occurs)**
- Merge `test2` into `test1`. Since both branches modified the same file, a merge conflict occurs.

- git merge test2


- output:

    ```
    CONFLICT (add/add): Merge conflict in task-04/ProgrammingLanuages.txt
    Automatic merge failed; fix conflicts and then commit the result.
    ```

The file now contains conflict markers:

```
Programming languages:
- Java
- Python
<<<<<<< HEAD
- Ruby
- JavaScript
=======
- PHP
- C/C++
>>>>>>> test2
```


### 5. **Resolve the Merge Conflict Manually**
We manually edit `ProgrammingLanuages.txt` to merge the changes correctly:

```
Programming languages:
- Java
- Python
- Ruby
- JavaScript
- PHP
- C/C++
```

After resolving the conflict, we stage the changes and commit.

- git commit -m "After Resolved the merge conflict Manually"


- Merge `test1` into `main` branch
