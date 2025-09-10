### Undoing Changes in Git

- **git revert <commit_id>**: Creates a new commit that undoes the changes introduced by a specific commit, while keeping all subsequent commits intact. This is safe for collaborative projects since it preserves history.
- **git reset <commit_id>**: Moves the branch back to the given commit and removes all commits after it. This rewrites history and should be used with caution (often requires `--force` when pushing).

In this exercise, I:
1. Created and committed `cv.md`, `address.md`, and `phone.md`.
2. Used `git revert` to undo the addition of `address.md` while keeping later commits.
3. Used `git reset` to roll back the repo to the initial commit, which removed all later commits.

