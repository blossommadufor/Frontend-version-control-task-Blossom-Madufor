# Frontend-version-control-task-Blossom-Madufor

# Frontend Version Control Task

## Project Overview
This project demonstrates collaborative Git and GitHub workflows, including repository initialization, feature branch isolation, structured multi-commit history, pull request code reviews, commit reversions, and branch renaming.

---

## Branching Strategy

| Branch Name | Purpose |
| :--- | :--- |
| `main` | Primary production branch containing fully merged code. |
| `feature-header` | Development branch used to create HTML navigation and header styling. |
| `feature-footer` | Development branch used to implement footer layout and social media links. |
| `feature-sidebar` | Created as `temp-sidebar-branch` and renamed using `git branch -m` to demonstrate branch management. |

---

## Merged Pull Requests

### Header Feature PR
![Header PR Screenshot](./screenshots/pr-header.png)

### Footer Feature PR
![Footer PR Screenshot](./screenshots/pr-footer.png)

---

## Frequently Used Git Commands

- **Branch Management:** `git checkout -b <branch>`, `git branch -m <old-name> <new-name>`, `git branch`
- **Staging & Committing:** `git add <file>`, `git commit -m "message"`
- **Pushing & Syncing:** `git push -u origin <branch>`, `git pull origin main`, `git fetch --all`
- **Reverting Changes:** `git log --oneline`, `git revert HEAD --no-edit`

---

## Lessons Learned

1. **Branch Isolation:** Working in feature branches keeps the `main` code safe while new ideas are built and tested.
2. **Clear Commit Messages:** Writing clear commit prefixes like `feat:` or `style:` makes reviewing code history much faster for teams.
3. **Safe Reversions:** Using `git revert` is better than deleting commits because it maintains an accurate history of what was fixed and why.