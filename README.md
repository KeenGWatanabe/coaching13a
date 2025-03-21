No, you did not perform the correct action based on the sentence you provided. The command `git pull origin feature` updates your **current branch** with the latest changes from the `feature` branch on the remote repository. It does not merge the `feature` branch into the `main` branch.

Here’s what you need to do to create a pull request to merge changes from the `feature` branch into the `main` branch:

---

### Steps to Create a Pull Request:
1. **Ensure your `feature` branch is up to date:**
   ```bash
   git checkout feature
   git pull origin feature
   ```

2. **Push your `feature` branch to the remote repository (if not already done):**
   ```bash
   git push origin feature
   ```

3. **Go to GitHub:**
   - Navigate to your repository on GitHub.
   - You should see a prompt to create a pull request for the `feature` branch. If not, click on the "Pull Requests" tab and then click "New Pull Request."

4. **Create the Pull Request:**
   - Set the **base branch** to `main` (the branch you want to merge into).
   - Set the **compare branch** to `feature` (the branch with your changes).
   - Add a title and description for the pull request.
   - Click "Create Pull Request."

---

### If You Want to Merge Locally:
If you want to merge the `feature` branch into `main` locally (without using GitHub's pull request feature), follow these steps:

1. **Switch to the `main` branch and update it:**
   ```bash
   git checkout main
   git pull origin main
   ```

2. **Merge the `feature` branch into `main`:**
   ```bash
   git merge feature
   ```

3. **Push the updated `main` branch to the remote repository:**
   ```bash
   git push origin main
   ```

---

### Key Points:
- `git pull` is used to fetch and merge changes from a remote branch into your current branch. It does not create a pull request or merge branches automatically.
- A pull request is a GitHub (or Git hosting service) feature to propose and review changes before merging.
- If you want to merge branches locally, use `git merge` after ensuring both branches are up to date.

Let me know if you need further clarification!