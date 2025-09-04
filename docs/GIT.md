# Git Workflow
## Branch Naming Scheme
All changes should be developed in a new branch created from the main branch.
Branches use the following naming conventions:
- `feat/{something}` -- When you are adding a completely new feature.
- `fix/{something}` -- When you are fixing something broken.
- `refactor/{something}` -- When you are improving the structure of the code without changing behavior.
- `docs/{something}` -- When you are making changes to documentation.
- `try/{something}` -- When you are experimenting with an idea and want feedback.
For example, you can run: `git checkout main` and then `git checkout -b fix/robot-movement` to create a new `fix/robot-movement` branch.
## Mind Your Commits
- [Commit Early, Commit Often](https://sethrobertson.github.io/GitBestPractices/); small, logical commits are easier to review.
- Ensure that your commit messages are [meaningful and follow a convention](https://www.conventionalcommits.org/).
## Keeping Your Branch Up To Date
As you work, the main branch may be updated by other contributors. It's important to keep your feature branch up-to-date with the latest changes from main.
1. **Rebase (Preferred):** Rebasing is the preferred method for updating your branch. It rewrites your branch's history to appear as if you started your work from the latest version of `main`, resulting in a clean, linear history.
  ```bash
  # Make sure your local main is up to date
  git checkout main
  git pull origin main

  # Switch back to your feature branch
  git checkout feat/my-new-feature

  # Rebase your branch on top of main
  git rebase main
  ```

  You may need to resolve conflicts during a rebase. If you have already pushed your branch to the remote, you will need to force-push your changes after rebasing:
  
  ```bash
  # Be careful! This rewrites history on the remote branch.
  git push --force-with-lease
  ```

2. **Merge:** You can also merge `main` into your branch. This is simpler but results in an extra "merge commit" in your branch's history.

  ```bash
  # Make sure your local main is up to date
  git checkout main
  git pull origin main

  # Switch back to your feature branch
  git checkout feat/my-new-feature

  # Merge main into your branch
  git merge main
  ```

Generally, prefer **rebasing** for keeping your feature branches updated, and use **merging** for bringing pull requests into the main branch.
