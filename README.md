## ITI Git Lab 2 - Version Control System

This repository documents the completion of Git Lab 2, covering branching strategies, merging, version tagging, and file management.

---

## 1. Repository Setup & Configuration
The repository was initialized and the default branch was renamed from `master` to `main`.

* **Initialize Local Repository**: `git init`
* **Rename Branch**: `git branch -m main`
* **Set Identity**: 
    ```bash
    git config --global user.name "Tarek Abdelrahman"
    git config --global user.email "tarekabdelrahman2002@gmail.com.com"
    ```

---



## 2. Branching & Feature Work
Two feature branches were created to manage development and testing independently.

**Create dev branch:**  `git checkout -b dev`
**Create test branch:** `git checkout -b test`

Push Branches:

```Bash
git push origin dev
git push origin test
```
---

## 3. Merging & Integration
All features were consolidated into the primary branch.

* **Merge dev**: `git checkout main` then `git merge dev`
* **Merge test**: `git merge test` (Triggered a merge commit via the 'ort' strategy).
* **Final Push**: `git push origin main`

---

## 4. How to Remove Branches
* **Remove Locally**: `git branch -d dev`
* **Remove Remotely**: `git push origin --delete dev`

---

## 5.  How to Checkout Without Committing
To switch branches while having uncommitted work, we use the **Stash** area:
1.  **Save progress**: `git stash`
2.  **Switch branch**: `git checkout <other_branch>`
3.  **Restore progress**: `git stash pop` (when returning to the original branch).

---

## 6. Tagging & Versioning
Annotated tags were used to mark the completion of the lab.

* **Create Annotated Tag**: `git tag -a v1.7 -m "version 1.7"`
* **Push Tag to Remote**: `git push origin v1.7`
* **List Tags**: `git tag`
* **Delete Tag Locally:** `git tag -d v1.7`
* **Delete Tag Remotely:** `git push origin --delete v1.7`

<img width="596" height="226" alt="image" src="https://github.com/user-attachments/assets/2705cf95-ee32-41ab-b2d0-3ff03ac6aa6a" />

---

## 7. Lab Architecture Image
The following diagram represents the workflow and branching strategy used during this lab.

* **Add Image to README**: 
    ```markdown
    ![Git Workflow Diagram](./images/image.png)
    ```

<img width="474" height="210" alt="image" src="https://github.com/user-attachments/assets/e9c9a9ba-029f-4404-bab5-d944642fc864" />




